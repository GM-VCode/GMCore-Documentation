# Políticas funcionais do GM Core

Esta pasta reúne documentos públicos de governança das funções sensíveis do GM Core. Eles explicam
finalidade, funcionamento, dados utilizados, acesso e limites. Detalhes de operação dos comandos
continuam em [`docs/comandos`](../comandos/README.md).

## Estado dos recursos

- **Operacional:** disponível no bot e sujeito às regras descritas.
- **Parcial:** disponível, mas algumas integrações dependem da configuração do servidor.
- **Em crescimento:** possui uma base funcional, mas ainda recebe evolução de governança e cobertura.
- **Em desenvolvimento:** opcional, experimental ou ainda não tratado como serviço estável.

## Índice

| Documento | Escopo | Estado |
|---|---|---|
| [Privacidade e tratamento de dados](PRIVACIDADE_E_DADOS.md) | Visão geral dos dados usados pelo bot | Operacional |
| [Controle de acesso](CONTROLE_DE_ACESSO.md) | ACL, permissões nativas e equipe técnica | Operacional |
| [Moderação e punições](MODERACAO_E_PUNICOES.md) | Ban, kick, silenciamentos e registros | Operacional |
| [Histórico entre comunidades](HISTORICO_MODERACAO_ENTRE_COMUNIDADES.md) | Consulta restrita de ocorrências por ID | Em crescimento e desenvolvimento |
| [Auditoria da comunidade](AUDITORIA_DA_COMUNIDADE.md) | Eventos, mensagens, voz e retenção | Operacional |
| [Proteções e Anti-Raid](PROTECOES_E_ANTI_RAID.md) | Contas, conteúdo, links, spam, bots, Anti-Nuke e emergência | Operacional |
| [Tickets de suporte](TICKETS_DE_SUPORTE.md) | Atendimento, participantes e transcript | Operacional |
| [Notificações privadas](NOTIFICACOES_PRIVADAS.md) | Alertas administrativos por DM | Operacional |
| [Divulgação por mensagem direta](DIVULGACAO_POR_DM.md) | Campanhas administrativas por DM | Operacional |
| [Sistema VIP](SISTEMA_VIP.md) | Assinaturas, cargos, calls e acompanhantes | Operacional |
| [Gerador de embeds](GERADOR_DE_EMBEDS.md) | Modelos, versões e publicações | Operacional |
| [Joker IA](JOKER_IA.md) | Assistente opcional conectado a provedor externo | Em desenvolvimento |

## Regra de interpretação

Esses documentos descrevem o comportamento do GM Core. Eles não substituem as regras do Discord,
as regras de cada comunidade nem aconselhamento jurídico. Recursos novos devem atualizar a política
correspondente antes de serem apresentados como estáveis.
