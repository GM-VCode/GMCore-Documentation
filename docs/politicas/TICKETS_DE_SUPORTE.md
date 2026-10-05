# Tickets de suporte

## Finalidade

O Ticket de Suporte oferece atendimento privado. Ele está disponível a partir do Essencial; o
Ticket de Sorteio, a partir do Premium.

## Funcionamento

O usuário abre o atendimento por um painel público. O bot cria um tópico privado acessível ao autor,
à equipe responsável e ao próprio bot. Um integrante autorizado assume o ticket, pode incluir pessoas
e criar no máximo uma call privada sob demanda. O autor comum não pode finalizar o próprio ticket;
o atendente, um administrador nativo ou alguém com `TICKET_MANAGE` pode fazê-lo.

No Premium e Pro, o encerramento produz um relatório HTML enviado ao `TICKET_LOG`; esse canal
precisa estar disponível. No Essencial, o atendimento pode ser encerrado sem relatório. O tópico
é arquivado e sua exclusão pode ser liberada.

## Dados incluídos

O registro pode conter ID e nome de quem abriu, atendente, participantes adicionados, pessoas que
escreveram ou entraram na call, mensagens, horários e anexos referenciados no atendimento. O HTML é
um retrato da conversa, não uma cópia permanente mantida pelo banco do bot.

## Retenção e acesso

Os registros temporários do atendimento são mantidos por prazo limitado. O arquivo
enviado ao Discord permanece sob controle da comunidade e de suas regras de retenção. O tópico e o
canal de auditoria devem ser visíveis somente às pessoas autorizadas pela configuração do servidor.

## Limites

O GM Core não garante disponibilidade futura de anexos hospedados externamente ou removidos do
Discord. A comunidade é responsável por baixar e conservar o transcript quando precisar de uma cópia
fora do Discord.
