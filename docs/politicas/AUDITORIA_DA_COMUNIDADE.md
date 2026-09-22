# Auditoria da comunidade

## Finalidade

A auditoria registra acontecimentos relevantes do servidor para permitir investigação, restauração
de contexto e responsabilização administrativa.

## Eventos cobertos

Conforme os canais configurados e os eventos entregues pelo Discord, o sistema trata alterações de
servidor, canais, cargos, membros, mensagens, convites, webhooks, emojis, stickers, voz, eventos,
integrações, AutoMod e outras entradas do Audit Log. Também registra entradas e saídas de membros,
edições ou exclusões de mensagens e sessões de voz observadas pelo Gateway.

O conteúdo de uma mensagem pode ser mantido em cache para que uma edição ou exclusão seja explicada.
O sistema deduplica eventos e tenta correlacionar a ação com o executor informado pelo Audit Log.

## Acesso e destino

Os registros são enviados somente aos canais de auditoria configurados no servidor. Consultas
persistentes exigem autorização administrativa ou capacidade interna compatível e são exibidas de
forma privada. Canais ausentes podem direcionar o evento ao canal geral de fallback.

## Retenção e resiliência

Os registros principais persistentes expiram em 45 dias. Coleções auxiliares podem expirar em 7 dias,
o histórico consolidado de membro após 60 dias sem atualização e o cache persistente de mensagens em
90 dias. Em memória, existe um cache circular limitado por canal e uma fila limitada; em saturação,
o item mais antigo pode ser descartado.

Falha no MongoDB não deve derrubar o listener nem impedir, quando possível, o envio do registro ao
Discord. Mesmo assim, permissões insuficientes, eventos não entregues pelo Gateway e mensagens não
presentes no cache podem produzir registros incompletos.

## Separação do histórico entre comunidades

A auditoria geral é interna ao servidor. A única visualização entre comunidades é a consulta restrita
de ocorrências de moderação descrita em
[`HISTORICO_MODERACAO_ENTRE_COMUNIDADES.md`](HISTORICO_MODERACAO_ENTRE_COMUNIDADES.md); ela não abre
os logs internos, mensagens ou identidade do moderador de outra comunidade.
