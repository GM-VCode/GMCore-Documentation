# Notificações privadas

## Finalidade

As notificações privadas avisam pessoas autorizadas sobre eventos administrativos importantes sem
expor o alerta em canais públicos.

## Funcionamento

Cada usuário configura suas preferências por servidor. É possível ativar categorias de Anti-Raid,
bots, emergência e punições, definir níveis por categoria, ajustar o detector de punições em massa e
estabelecer horário silencioso. As preferências começam desativadas.

A categoria Anti-Raid inclui picos de entrada e incidentes confirmados pelo Anti-Nuke. O executor do
incidente não recebe a notificação sobre a própria ação.

O painel permite testar a DM e remover mensagens enviadas por esta instância do bot. A limpeza não
apaga mensagens de outros usuários ou aplicações.

## Dados utilizados e limites

O GM Core mantém ID do servidor, ID do usuário, categorias, níveis, limites e horário silencioso. O
bot não lê a caixa de entrada privada do usuário; ele apenas tenta enviar e, quando solicitado, percorre
a conversa com o próprio bot para excluir mensagens de sua autoria.

O recebimento depende das configurações de privacidade, bloqueios e disponibilidade do Discord. Uma
falha de DM é informada quando possível e não autoriza o uso de outro meio de contato.
