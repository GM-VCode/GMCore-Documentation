# GM Core

### Gestão, segurança e governança para comunidades Discord

O **GM Core** é um sistema completo de administração para comunidades Discord. Seu objetivo é ajudar
equipes responsáveis a manter ambientes organizados, seguros e saudáveis, reduzindo abuso, spam,
toxicidade e falhas de comunicação sem retirar das pessoas a responsabilidade pelas decisões.

> **Nosso compromisso com o cliente:** o GM Core é desenvolvido para entregar **conforto** na
> administração diária, **segurança** contra abusos e incidentes e **governança** para que cada
> comunidade mantenha controle claro sobre seus responsáveis, regras, dados e decisões.

Mais do que reunir comandos de moderação, o GM Core conecta proteção, atendimento, auditoria,
controle de acesso e gestão da comunidade em uma única estrutura.

> Tecnologia para apoiar comunidades melhores — com regras claras, registros verificáveis e decisões
> humanas.

## Por que o GM Core existe

Administrar uma comunidade envolve muito mais do que banir ou silenciar usuários. É necessário saber
quem pode executar cada ação, preservar registros importantes, organizar atendimentos, responder a
incidentes e evitar que ferramentas administrativas sejam usadas sem controle.

O GM Core foi criado para oferecer essa base:

- reduzir comportamentos abusivos e conteúdo indesejado;
- prevenir ataques, spam e entradas suspeitas;
- organizar o trabalho das equipes de administração e moderação;
- registrar ações relevantes para consulta e responsabilização;
- oferecer atendimento privado e documentado aos membros;
- delegar funções sem entregar acesso irrestrito;
- manter cada comunidade no controle de suas próprias regras.

## Pilares do sistema

### Segurança preventiva

As proteções do GM Core podem identificar contas muito recentes, palavras negadas, links não
autorizados, mensagens repetidas, excesso de menções, bots não permitidos, picos de entrada e abuso
repetido de ações administrativas perigosas.

Cada proteção começa desativada. O responsável escolhe quais recursos deseja utilizar e configura os
limites adequados à realidade de sua comunidade.

Em situações graves, o modo de emergência permite proteger canais previamente definidos, aplicar
modo lento e acionar recursos nativos de segurança do Discord quando disponíveis.

### Moderação responsável

Banimentos, expulsões e silenciamentos passam por verificações de acesso, hierarquia e permissões do
Discord. Motivo, duração e informações essenciais da ocorrência podem ser registrados para permitir
revisão posterior.

O histórico oferece contexto, não uma sentença automática. O GM Core não atribui pontuação de risco e
não obriga uma comunidade a repetir a decisão tomada por outra. A análise final continua sendo humana.

### Governança e controle de acesso

O sistema possui uma camada própria de permissões por servidor. O dono pode autorizar uma pessoa ou
cargo somente para a função necessária, como tickets, embeds, VIP, Anti-Link ou auditoria, sem
entregar acesso completo ao bot.

As permissões internas complementam — e nunca ignoram — a hierarquia, os cargos e as restrições do
Discord. Alterações de acesso também podem ser auditadas.

### Auditoria e transparência

O GM Core acompanha eventos administrativos relevantes, como alterações em canais e cargos,
moderação de membros, edição ou exclusão de mensagens e movimentações de voz, conforme as permissões
e configurações da comunidade.

Os registros são direcionados a canais protegidos e possuem retenção controlada. A auditoria existe
para esclarecer acontecimentos e apoiar a equipe responsável, não para vigiar indiscriminadamente os
membros.

### Atendimento organizado

O sistema de tickets cria um espaço privado entre o membro e a equipe de suporte. Um atendente pode
assumir o caso, incluir participantes e criar uma call privada somente quando necessário.

Ao finalizar, o GM Core produz um transcript HTML e o envia ao canal de auditoria configurado. Isso
preserva o registro do atendimento sem manter indefinidamente toda a conversa no banco do bot.

### Comunicação e identidade

O Gerador de Embeds permite criar conteúdo visual, salvar modelos, manter versões e publicar somente
em canais autorizados. A divulgação por DM possui controle de acesso, confirmação, fila e respeito às
limitações impostas pelo Discord.

O sistema VIP administra cargos temporários, calls particulares, tags pessoais e acompanhantes. O GM
Core cuida da estrutura técnica; pagamentos e regras comerciais permanecem sob responsabilidade da
comunidade.

## Recursos principais

| Área | Recursos |
|---|---|
| Moderação | Ban, unban, kick, timeout de chat, mute de voz e remoção de mute |
| Proteção | Contas recentes, palavras negadas, Anti-Link, Anti-Spam, Anti-Nuke e bots autorizados |
| Resposta a incidentes | Monitoramento administrativo e modo de emergência |
| Auditoria | Eventos do servidor, histórico de membros, mensagens e voz |
| Governança | Permissões internas por usuário ou cargo e centrais administrativas |
| Atendimento | Tickets privados, atendente, call sob demanda e transcript |
| Conteúdo | Gerador de embeds, modelos, versões e publicações registradas |
| Comunicação | Notificações administrativas e divulgação por DM |
| Comunidade | Cargos VIP, calls privadas, tags e acompanhantes |
| Continuidade | Comandos essenciais de contingência durante falhas do serviço principal |

## Privacidade por finalidade

O GM Core utiliza identificadores fornecidos pelo Discord e informações necessárias ao funcionamento
dos recursos ativados. O sistema não solicita senhas, tokens de conta, documentos civis ou dados
bancários.

Os dados são separados por servidor sempre que a função assim exige. Consultas e painéis sensíveis
ficam restritos a pessoas autorizadas. Diferentes categorias de registro possuem prazos de retenção
próprios, evitando que dados temporários permaneçam armazenados sem necessidade operacional.

O histórico de moderação entre comunidades possui finalidade limitada: apresentar a equipes
autorizadas a punição, o motivo, a comunidade, a data e a duração aplicável. Ele não expõe mensagens,
anexos, denunciantes ou a identidade de quem aplicou a medida. Esse recurso está em crescimento e
desenvolvimento, podendo receber ajustes de governança e cobertura antes de ser considerado
plenamente estabilizado.

## Princípios de governança

O desenvolvimento e a operação do GM Core seguem princípios simples:

1. **Controle da comunidade:** cada servidor escolhe suas proteções, responsáveis e limites.
2. **Menor acesso necessário:** uma pessoa recebe somente as capacidades exigidas por sua função.
3. **Decisão humana:** registros e alertas apoiam a equipe, mas não substituem análise contextual.
4. **Rastreabilidade:** operações sensíveis devem produzir evidências adequadas quando possível.
5. **Minimização:** o bot registra apenas o necessário para entregar a função configurada.
6. **Separação:** dados, permissões e configurações de uma comunidade não liberam acesso em outra.
7. **Respeito à plataforma:** nenhuma permissão interna ultrapassa os limites da API do Discord.

## Responsabilidade compartilhada

O GM Core fornece infraestrutura, controles e registros. A comunidade continua responsável por suas
regras, pela escolha de pessoas autorizadas, pela proporcionalidade das punições e pelo conteúdo que
publica ou envia.

O bot não substitui os mecanismos oficiais de denúncia do Discord, serviços de emergência,
investigações formais ou orientação jurídica. Situações graves devem ser encaminhadas pelos meios
apropriados.

## Desenvolvimento contínuo

O GM Core evolui de forma modular. Recursos estáveis são documentados conforme o comportamento real;
recursos parciais ou experimentais são identificados antes de serem apresentados como concluídos.

O **Joker IA** é opcional e permanece em desenvolvimento. O **Anti-Nuke** já integra as proteções
operacionais, mas nasce desativado e depende de configuração exclusiva do dono real do servidor.
Essas distinções evitam que propostas futuras sejam confundidas com garantias do sistema atual.

## Compromisso

O GM Core busca tornar a gestão de comunidades mais previsível, segura e transparente. Seu papel não
é controlar as pessoas, mas oferecer às equipes responsáveis ferramentas para prevenir abuso,
responder a incidentes, organizar decisões e construir ambientes em que os membros possam participar
com mais confiança.

---

**GM Core** — gestão e governança para comunidades que levam segurança, organização e convivência a
sério.

Consulte as [políticas funcionais e de dados](docs/politicas/README.md) para conhecer em detalhes a
finalidade, o acesso, a retenção e os limites de cada sistema.
