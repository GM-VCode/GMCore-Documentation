# Auditoria da comunidade

## Finalidade

A auditoria registra acontecimentos relevantes do servidor para permitir investigação, restauração
de contexto e responsabilização administrativa.

## Eventos cobertos

Conforme os canais configurados e os eventos entregues pelo Discord, o sistema trata alterações de
servidor, canais, cargos, membros, mensagens, convites, webhooks, emojis, stickers, voz, eventos,
integrações, AutoMod e outras entradas do Audit Log. Também registra entradas e saídas de membros,
edições ou exclusões de mensagens e sessões de voz informadas pelo Discord.

Quando disponível, o registro de edição ou exclusão pode incluir o conteúdo anterior da mensagem e
o executor informado pelo Discord. Alguns eventos podem chegar incompletos ou sem identificação.

## Acesso e destino

Os registros são enviados somente aos canais de auditoria configurados no servidor. Consultas
persistentes exigem autorização administrativa ou capacidade interna compatível e são exibidas de
forma privada. Canais ausentes podem direcionar o evento ao canal geral de fallback.

## Retenção e resiliência

Os registros têm prazos de retenção diferentes conforme a finalidade, descritos na
[política de privacidade](PRIVACIDADE_E_DADOS.md). Eventos indisponíveis, falta de permissões ou
limitações do Discord podem deixar o registro incompleto.

Uma indisponibilidade do serviço pode limitar a consulta ou o envio dos registros. Não se deve
interpretar a ausência de um evento como prova de que ele não ocorreu.

## Separação do histórico entre comunidades

A auditoria geral é interna ao servidor. A única visualização entre comunidades é a consulta restrita
de ocorrências de moderação descrita em
[`HISTORICO_MODERACAO_ENTRE_COMUNIDADES.md`](HISTORICO_MODERACAO_ENTRE_COMUNIDADES.md); ela não abre
os logs internos, mensagens ou identidade do moderador de outra comunidade.
