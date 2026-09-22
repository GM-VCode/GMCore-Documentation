# Moderação e punições

## Finalidade

Os comandos de moderação permitem aplicar banimento, desbanimento, expulsão, timeout de chat,
silenciamento de voz e remoção de silenciamento com motivo e controle de acesso.

## Funcionamento

Antes da execução, o GM Core verifica a capacidade exigida, o servidor, a hierarquia entre membros,
a posição do cargo do bot e as permissões nativas necessárias. O timeout de chat utiliza o recurso
nativo do Discord e aceita duração entre 5 segundos e 28 dias. Registros persistentes permitem
reaplicar um timeout ainda válido quando o membro retorna ao servidor.

Os comandos de contingência por prefixo oferecem somente ações essenciais quando o MongoDB ou os
slash commands estão indisponíveis. Eles usam um armazenamento SQLite mínimo e não substituem a
auditoria completa.

## Registros

Uma ocorrência pode conter ID e nome do membro, servidor, ação, motivo, data, duração e estado. O
responsável é preservado na auditoria interna, mas não é apresentado na consulta entre comunidades.
Esses dados existem para continuidade operacional, revisão humana e prestação de contas.

## Limites e responsabilidade

O GM Core executa a decisão de uma pessoa autorizada ou uma proteção previamente ativada. O histórico
não gera pontuação de risco, não condena automaticamente o membro e não substitui a análise da equipe
da comunidade. Uma punição aplicada em um servidor não é automaticamente aplicada em outro.
