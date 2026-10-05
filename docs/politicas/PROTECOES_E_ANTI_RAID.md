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
- **Anti-Nuke:** detecta padrões de ações administrativas perigosas, pode conter o abuso nos limites
  das permissões do bot e registra o incidente para revisão humana.
- **Monitoramento da staff:** observa volume de ações administrativas e informa responsáveis.
- **Modo de emergência:** bloqueia ou aplica modo lento somente nos canais cadastrados, eleva a
  verificação quando possível e tenta pausar convites temporariamente.

## Dados utilizados

São mantidas as configurações, exceções e informações necessárias às proteções ativadas. Alertas
e incidentes relevantes podem ser enviados aos canais de auditoria configurados.

## Limites

O sistema trabalha com regras objetivas e pode produzir falso positivo. Responsáveis devem escolher
limites proporcionais e revisar os logs. O monitoramento da staff gera sinalização; não substitui
governança humana. O modo de emergência afeta apenas canais definidos e conserva o estado anterior
para restauração; falhas parciais são informadas no painel.

O Anti-Nuke reage depois que o Discord disponibiliza o evento e não restaura objetos já
apagados. Está disponível desde o Essencial e pode ser configurado pelo dono ou co-dono autorizado.
A contenção depende da hierarquia de cargos do bot e nunca bane,
expulsa ou aplica timeout automaticamente.
