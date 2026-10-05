# `/proprietario`

Centraliza configurações estruturais e sensíveis do servidor.

## Uso

```text
/proprietario painel:<opção>
```

## Opções e capacidades

| Opção | Função | Capacidade |
|---|---|---|
| Proteção de contas e Anti-Raid | Abre a central de proteção | Capacidade do módulo; Anti-Nuke desde o Essencial |
| Monitoramento da staff | Alvos, limites e alertas de ações sensíveis | `STAFF_MONITOR_MANAGE` |
| Modo de emergência | Bloqueio temporário e restauração dos canais | `EMERGENCY_MANAGE` |
| Divulgação | Campanhas de eventos por DM | `DIVE` |
| Configuração do servidor | Canais de auditoria, cargo padrão, XP em voz e backup | Conforme a ferramenta |
| Administração VIP | Cargos, categorias, concessões e remoções | `VIP_MANAGE` |

O dono do servidor, a equipe técnica, o co-dono com `PROPRIETARIO` ou a capacidade unitária
correspondente podem abrir as opções permitidas pelo plano. Administrador nativo não recebe acesso
automático a esta central.

## Pontos importantes

- O provisionamento de auditoria pode criar canais específicos para tickets e Anti-Nuke.
- `Configuração do servidor` reúne canais de auditoria, cargo padrão, XP em voz e backup.
- A divulgação possui filtro de conteúdo, lotes, cooldown e retomada.
- O modo de emergência guarda o estado necessário para restaurar os canais.
- `Bot-Moderação` fica dentro da central Moderação GM, exige `BOT_WHITELIST_MANAGE` e reutiliza o
  painel de whitelist e proteção de bots.
- Entrar na central não libera todos os seus módulos: contas, palavras e bots conferem suas
  capacidades unitárias antes de abrir.
- A proteção de bots aprende os bots existentes antes de ser ativada.
- Anti-Link possui painel próprio e exige `ANTI_LINK_MANAGE`.
- Anti-Spam possui painel próprio e exige `ANTI_SPAM_MANAGE`.
- Anti-Spam detecta repetição, similaridade, excesso configurável de menções e flood de símbolos.
- Moderação de palavras permite configurar timeout entre 5 segundos e 28 dias ou desativá-lo.
- Os painéis abertos pela central usam containers com seus botões e listas integrados.
- Todas as proteções nascem desligadas e precisam de ativação explícita.
- Anti-Nuke possui limites configuráveis por ação e restauração dos padrões.
- Anti-Nuke monitora bans, kicks, canais, cargos, webhooks, bots, prune e concessões perigosas por
  executor; a contenção remove somente cargos perigosos que o bot consegue administrar.
- Incidentes Anti-Nuke são registrados em `ANTI_NUKE_LOG`; a DM depende da preferência Anti-Raid de
  cada moderador no sistema de notificações.
- O dono real, co-dono delegado ou equipe técnica podem configurar Anti-Nuke se o plano o incluir.
- A administração VIP é separada do painel pessoal `/vip`.
- Monitoramento da staff e modo de emergência estão disponíveis a partir do Premium; campanhas
  por DM, no Pro. A administração VIP começa no Premium.
