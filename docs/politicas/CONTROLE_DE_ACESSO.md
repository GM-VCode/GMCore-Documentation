# Controle de acesso

## Finalidade

O controle de acesso restringe operações sensíveis e permite que o dono delegue apenas as funções
necessárias. O servidor precisa ter um plano ativo, inclusive o Gratuito. O plano disponibiliza
as ferramentas; a autorização do usuário e as permissões nativas do Discord determinam o acesso.

## Funcionamento

A ACL associa uma capacidade a um usuário ou cargo dentro de um servidor. A autorização considera o
dono, exceções técnicas documentadas, capacidades diretas e capacidades herdadas dos cargos. A ação
ainda depende da hierarquia, do acesso aos canais e das permissões do próprio bot.

O `/config` permite conceder, remover e listar acessos. A permissão unitária para editar a ACL é
concedida a usuários; `PROPRIETARIO` é uma delegação ampla de co-dono e também permite administrar
o acesso dentro do servidor. Nenhuma dessas permissões libera benefícios fora do plano.

## Dados registrados

As concessões e alterações de acesso ficam vinculadas ao servidor e podem ser auditadas.

## Equipe técnica

A equipe técnica oficial possui acesso para manutenção e testes dentro das ferramentas disponíveis
no plano do servidor. A equipe comercial recebe somente as funções de gestão de planos; ela não
herda autoridade de moderação ou configuração da comunidade.

## Limites

A ACL concede acessos positivos; não existem regras internas explícitas de negação, validade por
horário ou escopo por canal. Cada servidor administra suas próprias concessões, e uma concessão não é
transportada para outra comunidade.
