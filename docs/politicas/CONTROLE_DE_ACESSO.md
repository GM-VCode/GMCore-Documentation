# Controle de acesso

## Finalidade

O controle de acesso restringe operações sensíveis e permite que o dono delegue apenas as funções
necessárias. O GM Core combina permissões nativas do Discord com uma ACL própria por servidor.

## Funcionamento

A ACL associa uma capacidade a um usuário ou cargo dentro de um servidor. A autorização considera o
dono, exceções técnicas documentadas, capacidades diretas e capacidades herdadas dos cargos. A ação
ainda depende da hierarquia, do acesso aos canais e das permissões do próprio bot.

O `/config` permite conceder, remover e listar acessos. A capacidade que administra a própria ACL é
concedida somente a usuários, não a cargos. Se o banco não puder ser consultado, o acesso interno é
negado por segurança.

## Dados registrados

São mantidos o servidor, o alvo, o tipo do alvo, as capacidades, a data e a identidade de quem fez a
alteração. Nomes servem para exibição; IDs são a referência permanente. As mudanças entram na
auditoria administrativa.

## Equipe técnica

IDs oficiais configurados para suporte técnico podem possuir autoridade global no bot. Essa exceção
serve à manutenção e não altera a hierarquia do Discord. Os IDs devem permanecer restritos, e ações
administrativas continuam sujeitas aos registros disponíveis.

## Limites

A ACL concede acessos positivos; não existem regras internas explícitas de negação, validade por
horário ou escopo por canal. Cada servidor administra suas próprias concessões, e uma concessão não é
transportada para outra comunidade.
