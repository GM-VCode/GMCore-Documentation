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
- conteúdo de tickets, participantes e, nos planos com relatório, transcript de encerramento;
- modelos e publicações criados no Gerador de Embeds;
- estruturas e vínculos do sistema VIP;
- progresso temporário de campanhas por DM;
- tempo válido em voz, XP e progresso de membros e da staff nos servidores que usam esses recursos;
- informações necessárias à ativação, duração e gestão do plano do servidor.

O bot não solicita senha nem token de conta. Comprovantes enviados para ativação de planos podem
conter dados pessoais ou de pagamento; envie apenas o necessário e não inclua informações
sensíveis adicionais. O ID do Discord identifica contas mesmo quando nomes e apelidos mudam.

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
- dados usados para contextualizar edições e exclusões de mensagens podem ser mantidos por até
  90 dias;
- tickets encerrados e seus resumos diários expiram em 7 dias;
- eventos funcionais de VIP expiram em 2 dias;
- configurações, permissões, punições vigentes, modelos de embed e estruturas VIP permanecem enquanto
  forem necessários ao funcionamento ou até remoção administrativa. Após período prolongado sem
  plano ativo, as configurações do servidor podem ser redefinidas conforme os termos do serviço;
  registros necessários ao histórico entre comunidades podem permanecer.

A exclusão automática pode ocorrer pouco depois do prazo previsto. O transcript enviado ao canal
de auditoria passa a ser uma mensagem do próprio servidor e
segue a retenção administrada pela comunidade no Discord.

## Limites

O GM Core depende da API e das permissões concedidas pelo Discord. Falhas de acesso, indisponibilidade
do banco ou remoção de canais podem limitar registros. O bot não vende dados, não produz perfil
publicitário e não usa o conteúdo das comunidades para conceder punições automáticas fora das regras
explicitamente ativadas pelo servidor.

## Contato e suporte

Para dúvidas, solicitações ou relatos sobre privacidade e dados, entre em contato pelos canais
oficiais do GM Core:

- **Suporte:** [gmcore.help@outlook.com](mailto:gmcore.help@outlook.com)
- **Parcerias:** [gmcore.team@outlook.com](mailto:gmcore.team@outlook.com)
- **Servidor de suporte:** [discord.gg/wrTMNUUwFa](https://discord.gg/wrTMNUUwFa)
