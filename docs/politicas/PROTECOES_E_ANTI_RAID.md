# Proteções e Anti-Raid

## Estado

O conjunto é **operacional**: contas, palavras, Anti-Link, Anti-Spam, bots, Anti-Nuke,
monitoramento da staff e modo de emergência estão disponíveis. Todas as proteções começam
desativadas e dependem de ativação explícita do responsável.

## Finalidade e funcionamento

- **Moderação de entrada:** compara a idade da conta, aceita exceções e detecta picos de entrada.
- **Palavras negadas:** remove conteúdo configurado e pode aplicar timeout definido pelo servidor.
- **Anti-Link:** bloqueia links, com lista de usuários e cargos permitidos.
- **Anti-Spam:** considera repetição, semelhança, janela de tempo, excesso de menções e padrões de
  símbolos, podendo remover mensagens e aplicar timeout.
- **Bot-Moderação:** controla a entrada de bots por uma lista autorizada.
- **Anti-Nuke:** conta ações administrativas por executor em janelas rápida, intermediária e
  acumulada. Ao atingir um limite, remove do executor os cargos perigosos que o GM Core consegue
  administrar, registra o incidente em canal exclusivo e notifica somente os responsáveis que
  ativaram a categoria Anti-Raid no `/notificacoes`.
- **Monitoramento da staff:** observa volume de ações administrativas e informa responsáveis.
- **Modo de emergência:** bloqueia ou aplica modo lento somente nos canais cadastrados, eleva a
  verificação quando possível e tenta pausar convites temporariamente.

## Dados utilizados

São mantidas configurações por servidor, IDs das exceções, palavras configuradas, limites, duração de
timeout, listas de canais e o estado necessário para restauração. A detecção rápida de spam usa
amostras temporárias em memória; ela não cria um arquivo permanente com todas as mensagens analisadas.
O Anti-Nuke persiste apenas estado, janelas e limites. Seus contadores ficam em memória e o incidente
consolidado é enviado ao canal `ANTI_NUKE_LOG`, sem gravar cada incremento no banco.

## Limites

O sistema trabalha com regras objetivas e pode produzir falso positivo. Responsáveis devem escolher
limites proporcionais e revisar os logs. O monitoramento da staff gera sinalização; não substitui
governança humana. O modo de emergência afeta apenas canais definidos e conserva o estado anterior
para restauração; falhas parciais são informadas no painel.

O Anti-Nuke reage depois que o Discord entrega o evento do Audit Log e não restaura objetos já
apagados. Somente o dono real configura o recurso; o dono e o próprio GM Core são as únicas
exceções. Não há whitelist. A contenção depende da hierarquia de cargos do bot e nunca bane,
expulsa ou aplica timeout automaticamente.
