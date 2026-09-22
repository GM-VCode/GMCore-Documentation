# Privacidade e tratamento de dados

## Finalidade

O GM Core utiliza somente os dados necessários para executar moderação, auditoria, segurança,
atendimento e recursos configurados pela comunidade. O bot opera principalmente com identificadores
fornecidos pelo Discord e com conteúdo gerado dentro dos servidores em que está instalado.

## Dados utilizados

Conforme os módulos ativados, o bot pode tratar:

- IDs e nomes visuais de servidor, usuário, cargo, canal e mensagem;
- ações administrativas, punições, motivos, datas e durações;
- conteúdo de mensagens necessário à auditoria de edição ou exclusão;
- entrada, saída e movimentação em canais de voz;
- configurações, permissões internas e preferências de notificação;
- conteúdo de tickets, participantes e transcript produzido no encerramento;
- modelos e publicações criados no Gerador de Embeds;
- estruturas e vínculos do sistema VIP;
- progresso temporário de campanhas por DM.

O bot não solicita senha, token de conta, dados bancários ou documento civil. O ID do Discord é
usado como identificador técnico porque nomes e apelidos podem mudar.

## Isolamento e acesso

Configurações e registros operacionais são associados ao ID do servidor. Painéis sensíveis são
privados e protegidos por permissões nativas do Discord, pela ACL do GM Core ou por ambas. Uma
permissão interna não permite ultrapassar a hierarquia ou as restrições técnicas do Discord.

A exceção funcional é a consulta restrita do histórico de moderação entre comunidades, descrita em
documento próprio. Ela localiza ocorrências pelo ID informado e não expõe conversas ou o responsável
que aplicou a punição.

## Retenção

Não existe um prazo único para todos os dados:

- eventos principais de auditoria possuem expiração automática de 45 dias;
- algumas coleções auxiliares de logs expiram em 7 dias;
- o histórico consolidado de auditoria de membro expira após 60 dias sem atualização;
- cache persistente de mensagens possui expiração de 90 dias;
- tickets encerrados e seus resumos diários expiram em 7 dias;
- eventos funcionais de VIP expiram em 2 dias;
- configurações, permissões, punições vigentes, modelos de embed e estruturas VIP permanecem enquanto
  forem necessários ao funcionamento ou até remoção administrativa.

A exclusão por TTL é executada pelo MongoDB e pode ocorrer pouco depois do instante exato de
vencimento. O transcript enviado ao canal de auditoria passa a ser uma mensagem do próprio servidor e
segue a retenção administrada pela comunidade no Discord.

## Limites

O GM Core depende da API e das permissões concedidas pelo Discord. Falhas de acesso, indisponibilidade
do banco ou remoção de canais podem limitar registros. O bot não vende dados, não produz perfil
publicitário e não usa o conteúdo das comunidades para conceder punições automáticas fora das regras
explicitamente ativadas pelo servidor.
