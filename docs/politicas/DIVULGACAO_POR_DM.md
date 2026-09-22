# Divulgação por mensagem direta

## Finalidade

A divulgação permite que uma pessoa autorizada envie um aviso administrativo em formato de embed aos
membros não-bot do servidor.

## Funcionamento

A operação exige acesso próprio e confirmação do conteúdo. O envio ocorre gradualmente, respeita
limites e respostas da API do Discord e mantém um checkpoint para continuar depois de interrupções.
Bots são ignorados. Ao terminar, o solicitante recebe o resultado por DM e a ação entra no registro
administrativo.

## Dados utilizados

Durante uma campanha, o GM Core mantém servidor, solicitante, conteúdo do embed, IDs ainda pendentes,
contadores de envio, erros, ignorados, estado e datas. Esses dados servem à continuidade da campanha e
não formam uma lista comercial independente.

## Limites e responsabilidade

O envio pode falhar quando o membro bloqueia DMs, restringe mensagens do servidor ou quando o Discord
aplica limites. O recurso não contorna essas escolhas. A pessoa autorizada e a comunidade são
responsáveis pela legitimidade, frequência e conteúdo do aviso; o GM Core não deve ser usado para
spam, publicidade enganosa ou tentativa de evasão das regras do Discord.
