# Tickets de suporte

## Finalidade

O Ticket de Suporte oferece atendimento privado e um registro final verificável. O sistema atual
implementa somente o tipo Suporte.

## Funcionamento

O usuário abre o atendimento por um painel público. O bot cria um tópico privado acessível ao autor,
à equipe responsável e ao próprio bot. Um integrante autorizado assume o ticket, pode incluir pessoas
e criar no máximo uma call privada sob demanda. O autor comum não pode finalizar o próprio ticket;
o atendente, um administrador nativo ou alguém com `TICKET_MANAGE` pode fazê-lo.

Ao finalizar, o bot produz um transcript HTML, envia o arquivo ao canal `TICKET_LOG`, arquiva o tópico
e libera a exclusão. O encerramento é recusado quando o canal de log não está disponível, evitando a
perda silenciosa do registro.

## Dados incluídos

O registro pode conter ID e nome de quem abriu, atendente, participantes adicionados, pessoas que
escreveram ou entraram na call, mensagens, horários e anexos referenciados no atendimento. O HTML é
um retrato da conversa, não uma cópia permanente mantida pelo banco do bot.

## Retenção e acesso

O estado operacional encerrado e o resumo diário mínimo expiram do MongoDB após 7 dias. O arquivo
enviado ao Discord permanece sob controle da comunidade e de suas regras de retenção. O tópico e o
canal de auditoria devem ser visíveis somente às pessoas autorizadas pela configuração do servidor.

## Limites

O GM Core não garante disponibilidade futura de anexos hospedados externamente ou removidos do
Discord. A comunidade é responsável por baixar e conservar o transcript quando precisar de uma cópia
fora do Discord.
