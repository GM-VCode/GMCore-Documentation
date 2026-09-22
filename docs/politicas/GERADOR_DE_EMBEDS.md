# Gerador de embeds

## Finalidade

O Gerador de Embeds permite criar, revisar, versionar e publicar conteúdo visual pelo Discord sem
aceitar JSON arbitrário ou exigir ferramenta externa.

## Funcionamento

Uma sessão privada edita texto externo, título, descrição, links, aparência, autor, rodapé, campos e
botões de link. O usuário pode visualizar, salvar modelo, copiar, restaurar uma versão, arquivar e
publicar após confirmação. O GM Core só edita mensagens que ele próprio publicou e registrou.

## Dados e segurança

Modelos, versões, autor e vínculos de publicação são armazenados por servidor. URLs e limites do
Discord são validados; menções efetivas ficam desativadas por padrão; componentes não executam código
ou comandos arbitrários. Operações relevantes seguem para o canal funcional de conteúdo.

## Limites

O sistema trabalha com um embed por sessão e publicação, até 25 modelos ativos por servidor e os
limites de campos e componentes aceitos pelo Discord. As mensagens publicadas continuam como embeds
clássicos; os containers são usados nos painéis administrativos e não alteram o conteúdo final criado
pelo usuário.
