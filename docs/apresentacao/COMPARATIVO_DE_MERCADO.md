# GM Core em comparação com as principais soluções para Discord

> Comparativo funcional revisado em 22 de setembro de 2026. A avaliação considera recursos,
> integração, governança, segurança e experiência administrativa — não quantidade de servidores,
> tamanho da comunidade ou popularidade.

## Resumo executivo

O GM Core não foi criado para disputar somente uma lista de comandos. Ele reúne proteção,
moderação, auditoria, atendimento, conteúdo, gestão VIP e controle de acesso dentro de uma única
estrutura de governança.

Sua principal vantagem é a integração: a mesma identidade, a mesma ACL e a mesma lógica de auditoria
acompanham os diferentes módulos. Isso reduz permissões excessivas, configurações espalhadas e a
necessidade de combinar diversos bots para administrar uma comunidade.

### Avaliação atual

| Dimensão | Nota do GM Core | Leitura objetiva |
|---|---:|---|
| Governança e controle de acesso | **9,2/10** | Principal diferencial do produto |
| Auditoria e rastreabilidade | **8,8/10** | Muito competitivo entre soluções administrativas |
| Segurança e Anti-Raid | **8,1/10** | Forte e configurável; recuperação estrutural ainda não está disponível |
| Moderação | **8,2/10** | Operação sólida com histórico e validação de hierarquia |
| Tickets e atendimento | **7,7/10** | Fluxo completo de suporte, ainda com menor variedade que soluções especializadas |
| Embeds e comunicação | **8,5/10** | Editor integrado, modelos, versões e publicação controlada |
| Gestão de comunidade e VIP | **8,8/10** | Diferencial pouco comum em bots de segurança |
| Maturidade operacional | **7,0/10** | Produto funcional, entrando agora em experiência real com clientes |
| **Avaliação geral atual** | **8,2/10** | Forte como plataforma integrada de governança |

Essa nota não significa que o GM Core supera todos os concorrentes em suas especialidades. Wick
continua mais avançado em segurança extrema, Ticket Tool em variedade de tickets e Xenon em backup.
O GM Core se destaca por entregar essas áreas dentro de uma operação coerente e controlada.

## Soluções usadas como referência

- **Wick:** segurança, Anti-Nuke, quarentena, lockdown e resposta automatizada.
- **Dyno:** bot generalista com grande variedade de módulos, AutoMod e logs.
- **Carl-bot:** logging, cargos, reaction roles e automações comunitárias.
- **Ticket Tool:** atendimento especializado e altamente configurável.
- **Xenon:** backup, clonagem e restauração de estruturas do Discord.
- **Discord nativo:** AutoMod, timeout, Audit Log e permissões da plataforma.

## Segurança preventiva

| Recurso | GM Core | Mercado especializado | Diferencial do GM Core |
|---|---|---|---|
| Contas recentes | Idade mínima configurável e exceções controladas | Wick possui Gate e mecanismos de verificação | Integra a decisão ao painel geral de proteção |
| Pico de entradas | Detecta volume dentro de uma janela configurável | Wick oferece Anti-Raid e modos de pânico | Mitigação proporcional sem bloquear o servidor inteiro automaticamente |
| Palavras negadas | Filtro próprio com sincronização ao AutoMod quando disponível | Wick, Dyno e Discord possuem filtros equivalentes | Continua operando mesmo sem depender exclusivamente do AutoMod |
| Anti-Link | Bloqueio de URLs e convites com permissões por usuário ou cargo | Bots generalistas costumam oferecer filtros de links | Usa capacidade ACL própria e registra a operação no mesmo ecossistema |
| Anti-Spam | Repetição, semelhança, menções acumuladas e padrões excessivos de símbolos | Wick usa sistema de heat; Dyno e Discord possuem filtros de spam | Configuração simples, conservadora e adequada à carga do servidor |
| Bots não autorizados | Aprendizado inicial e lista de bots permitidos | Wick oferece filtros para entrada de bots | Administração integrada ao mesmo painel do Anti-Raid |
| Modo de emergência | Bloqueio ou modo lento em canais selecionados, com restauração do estado anterior | Wick possui lockdown e panic mode mais abrangentes | Atua somente no escopo escolhido pelo responsável |
| Ativação das proteções | Todos os módulos nascem desativados | Alguns concorrentes ativam proteções padrão durante o setup | A comunidade decide explicitamente o que o bot pode executar |

### Leitura da comparação

O Wick oferece uma camada de resposta extrema mais ampla, com quarentena, lockdown, verificação,
proteção contra tentativas de contornar a contenção e restauração associada a snapshots. O GM Core
prefere uma resposta menor e reversível: interrompe a autoridade perigosa, registra o incidente e
preserva o julgamento humano.

Essa escolha reduz automatismos agressivos, mas não substitui um sistema de backup. A recuperação de
estruturas apagadas é a principal capacidade ainda ausente para alcançar o nível mais alto de defesa.

## Anti-Nuke

| Capacidade | GM Core | Wick | Bots generalistas |
|---|---|---|---|
| Contagem por executor | Sim | Sim | Varia por produto |
| Janelas temporais | Rápida, intermediária e acumulada | Limites temporais e sistema de heat | Normalmente mais simples |
| Limites por ação | Sim, configuráveis | Sim, com grande granularidade | Cobertura variável |
| Banimentos e expulsões em massa | Detectados | Detectados | Nem sempre disponível |
| Exclusão e criação de canais/cargos | Detectadas | Detectadas | Geralmente limitada a logs |
| Webhooks | Alterações monitoradas | Criação e exclusão protegidas | Normalmente apenas auditadas |
| Prune | Detectado | Detectado | Pouco comum |
| Permissões perigosas | Concessão e entrega de cargos monitoradas | Proteção estrita de cargos e permissões | Pouco comum |
| Adição de bots | Detectada | Detectada | Varia |
| Resposta automática | Remove cargos perigosos administráveis | Quarentena e lockdown, conforme configuração | Geralmente punição simples ou alerta |
| Canal próprio de incidente | Sim | Logs próprios | Depende do bot |
| DM de alerta | Somente para quem aderiu à categoria | Alertas aos responsáveis | Varia |
| Imunidade | Somente dono real e GM Core | Sistema próprio de whitelist e permits | Varia |
| Configuração técnica | Dono ou equipe técnica global | Dono e autoridades configuradas | Administradores ou manager roles |
| Backup e restauração | Ainda não disponível | Disponível em planos e modos específicos | Normalmente inexistente |

### Onde o GM Core se destaca

- não usa uma whitelist ampla de pessoas imunes à detecção;
- separa autoridade para configurar de imunidade contra o detector;
- acompanha ações executadas por comandos do próprio bot até o solicitante humano;
- usa limites distintos para cada tipo de ação perigosa;
- conserva o estado desativado até a decisão explícita do responsável;
- integra incidentes ao sistema geral de auditoria e às preferências individuais de notificação.

## Governança e permissões

| Recurso | GM Core | Abordagem comum em outros bots |
|---|---|---|
| Permissão por capacidade | Cada módulo possui uma capacidade explícita | Muitos produtos trabalham com Administrador ou cargos gerenciais amplos |
| Concessão direta ou por cargo | Sim | Disponível de forma variável |
| Separação por servidor | Obrigatória em todas as concessões | Esperada, mas nem sempre exposta como política central |
| Capacidade ampla e unitária | Centrais completas ou somente uma função específica | Frequentemente baseada em acesso ao módulo inteiro |
| Gestão da própria ACL | `CONFIG_EDIT`, somente para usuário direto | Normalmente vinculada a Administrador ou Manage Server |
| Equipe técnica global | Autoridade separada do dono da comunidade | Suporte costuma depender do painel externo do fornecedor |
| Hierarquia do Discord | Continua obrigatória depois da ACL | Comportamento padrão da plataforma |
| Revogação em painel aberto | Revalidada em cada interação sensível | Nem sempre documentada |
| Falha do banco | Nega acesso e não confirma alteração | Comportamento raramente apresentado ao cliente |
| Registro de alterações | Integrado à auditoria administrativa | Dyno registra mudanças do dashboard; cobertura varia nos demais |

O diferencial não é apenas possuir permissões. É aplicar o princípio do menor acesso necessário em
todos os sistemas. Um responsável por tickets não precisa receber autoridade sobre VIP, Anti-Raid,
embeds ou configurações estruturais.

## Auditoria e responsabilização

| Recurso | GM Core | Concorrentes de referência |
|---|---|---|
| Eventos do Audit Log | Sim | Wick, Dyno e Carl-bot oferecem logs |
| Eventos do Gateway | Sim | Cobertura varia conforme o produto |
| Canais por finalidade | Criados e organizados pelo sistema | Carl-bot e outros permitem dividir logs |
| Identificação do executor | Correlação entre evento e executor real | Presente nos principais sistemas de log |
| Ações feitas pelo próprio bot | Relacionadas ao solicitante humano quando possível | Nem sempre aparece como identidade separada |
| Histórico de punições | Persistente e consultável | Dyno possui mod logs e casos |
| Histórico de membro | Consolida ocorrências relevantes | Varia por produto |
| Retenção por coleção | Controlada conforme finalidade | Nem sempre informada ao cliente |
| Notificações privadas | Adesão individual por servidor e categoria | Normalmente definidas de forma global pela administração |
| Auditoria entre comunidades | Em crescimento, com consulta restrita e dados mínimos | Não é um recurso comum entre bots generalistas |

O GM Core não usa auditoria somente como um fluxo de mensagens em canais. Os registros apoiam
consultas, responsabilização e continuidade operacional, respeitando a finalidade e a retenção de
cada categoria.

## Moderação

| Recurso | GM Core | Dyno/Wick/Discord |
|---|---|---|
| Ban, unban e kick | Sim | Sim |
| Timeout de chat | Usa o timeout nativo e registra vencimento | Disponível no Discord e nos principais bots |
| Mute de voz | Server mute com persistência temporal | Disponível nos principais bots |
| Reaplicação após retorno | Sim, enquanto a punição estiver ativa | Depende da implementação do produto |
| Motivo obrigatório | Sim nas ações relevantes | Configurável em alguns produtos |
| Proteção de administradores | Validação antes da ação | Hierarquia nativa também limita os concorrentes |
| Histórico consultável | Sim | Dyno e Wick oferecem registros de moderação |
| Decisão entre comunidades | Apenas contexto autorizado; nunca punição automática | Não é comum em bots generalistas |

O GM Core usa os mecanismos nativos do Discord sempre que eles representam a solução mais segura,
como timeout e server mute. A persistência do bot acrescenta histórico, expiração e reforço sem
recriar permissões canal por canal.

## Tickets e atendimento

| Recurso | GM Core | Ticket Tool |
|---|---|---|
| Painel público persistente | Sim | Sim |
| Atendimento privado | Tópico privado | Canais ou fluxos configuráveis |
| Atendente responsável | Um atendente assume o caso | Fluxos especializados e configuráveis |
| Participantes adicionais | Sim | Sim |
| Atendimento por voz | Call privada criada somente sob demanda | Depende da configuração e dos recursos do produto |
| Transcript | HTML enviado ao canal de auditoria | Transcripts fazem parte do produto especializado |
| Continuidade após reinício | Views persistentes | Sim |
| Integração com ACL | `TICKET_MANAGE` | Permissões próprias do sistema |
| Integração com auditoria geral | Nativa no GM Core | Voltada ao domínio de tickets |
| Minimização de dados | Estado temporário e resumo diário; transcript completo permanece no Discord | Política depende da configuração do serviço |
| Variedade de tipos | Suporte é o tipo atual | Ticket Tool possui maior variedade e personalização |

O Ticket Tool continua superior quando a prioridade exclusiva é construir muitos fluxos de
atendimento. O GM Core é mais interessante quando o ticket precisa compartilhar as mesmas regras de
acesso, auditoria e governança usadas no restante da comunidade.

## Conteúdo, comunicação e comunidade

| Recurso | GM Core | Referências de mercado | Diferencial |
|---|---|---|---|
| Gerador de embeds | Editor, modelos, versões, prévia e publicação registrada | Dyno possui Message Embedder; Carl-bot possui tags e automações | O GM Core controla também edição posterior e identidade da publicação |
| Components V2 | Painéis, botões, listas e textos dentro de containers | Adoção varia entre produtos | Experiência moderna diretamente no Discord |
| Divulgação por DM | Fila, confirmação e controle de acesso | Bots generalistas possuem anúncios e automações diversas | Operação integrada à governança do bot |
| Notificações administrativas | Preferência individual por servidor e categoria | Geralmente configuradas pela administração para canais ou grupos | Ninguém recebe DM administrativa sem ativar a própria preferência |
| Gestão VIP | Cargos temporários, calls, tags e acompanhantes | Não é foco dos bots de segurança | Une operação comercial da comunidade à governança técnica |
| Cargo padrão de entrada | Configurado com bloqueio de permissões perigosas | Autoroles são comuns em Dyno e Carl-bot | Validação de segurança antes da configuração |
| Contingência | Comandos essenciais mantidos em armazenamento local separado | Pouco visível nas ofertas públicas consultadas | Continuidade mínima quando o serviço principal está indisponível |

## Recuperação e continuidade

O Xenon é atualmente uma referência específica em backup. Sua documentação informa captura e
restauração de canais, cargos, categorias, permissões e configurações, com recursos adicionais para
mensagens, membros e snapshots automáticos em modalidades específicas.

O GM Core ainda não oferece restauração estrutural. Sua continuidade atual está concentrada em:

- estado persistente das configurações e punições;
- reaplicação de mutes ativos;
- views persistentes de tickets;
- restauração das alterações feitas pelo próprio modo de emergência;
- contingência local para comandos administrativos essenciais;
- auditoria que permite compreender o incidente.

Backup e restauração são a maior evolução necessária para que o GM Core dispute também o primeiro
nível de recuperação pós-incidente.

## Onde o GM Core fica acima dos bots generalistas

### 1. Governança integrada

Proteções, tickets, VIP, embeds, auditoria e moderação não possuem sistemas independentes de acesso.
Todos seguem capacidades explícitas e isoladas por servidor.

### 2. Menor privilégio como regra do produto

O responsável pode delegar apenas a função necessária. Isso é mais seguro que entregar
Administrador, Manage Server ou uma função gerencial ampla somente para operar um módulo.

### 3. Separação entre configurar e ficar imune

A equipe técnica pode prestar suporte no Anti-Nuke, mas continua sujeita à detecção. Autoridade de
manutenção não vira imunidade operacional.

### 4. Controle humano preservado

Alertas e históricos oferecem contexto. O GM Core evita transformar sinais em punições definitivas
quando uma revisão humana é mais apropriada.

### 5. Privacidade por adesão e finalidade

Notificações privadas são individuais e desativadas por padrão. Registros possuem finalidade,
escopo e retenção definidos, evitando coleta indiscriminada.

### 6. Sistemas comunitários no mesmo ecossistema

VIP, tickets, embeds e divulgação convivem com a segurança sem precisar entregar acesso amplo ou
instalar uma coleção de bots independentes.

### 7. Experiência dentro do Discord

As centrais usam containers, botões, listas e formulários. O cliente realiza as operações principais
sem depender de alternar constantemente entre o Discord e vários dashboards externos.

## Onde especialistas ainda estão à frente

- **Wick:** quarentena, verificação, panic mode, lockdown extremo e anos de especialização em
  segurança ofensiva e defensiva.
- **Dyno:** quantidade de módulos sociais, automações, feeds, níveis, formulários e dashboard.
- **Carl-bot:** reaction roles, tags e automações avançadas de cargos.
- **Ticket Tool:** variedade e profundidade de fluxos de atendimento.
- **Xenon:** snapshots, clonagem e restauração estrutural.

Essas diferenças não diminuem a proposta do GM Core. Elas mostram que ele compete como plataforma
integrada de gestão e governança, enquanto cada referência lidera uma especialidade.

## Posicionamento atual

O GM Core já pode ser apresentado como:

> Uma plataforma integrada de administração, segurança e governança para comunidades Discord, com
> controle granular de acesso, auditoria persistente, proteção configurável e ferramentas
> operacionais reunidas em uma única experiência.

Ele não deve ser anunciado como uma solução impenetrável nem como substituto absoluto de todos os
bots especializados. A afirmação mais sólida é que reduz fragmentação e oferece uma base de
governança mais coerente que a combinação casual de diversas ferramentas independentes.

## Fontes públicas consultadas

- [Wick — recursos e Anti-Nuke](https://docs.wick.bot/intro/features/)
- [Wick — configuração, limites e sistemas de proteção](https://docs.wick.bot/setup/)
- [Dyno — catálogo oficial de módulos](https://docs.dyno.gg/en/modules)
- [Dyno — logs administrativos](https://docs.dyno.gg/en/dashboard/logs)
- [Carl-bot — documentação de logging](https://github.com/botlabs-gg/carlbot-docs/blob/master/docs/logging.md)
- [Carl-bot — cargos e reaction roles](https://github.com/botlabs-gg/carlbot-docs/blob/master/docs/roles.md)
- [Ticket Tool — documentação oficial](https://docs.tickettool.xyz/)
- [Xenon — backups e restauração](https://xenon.bot/backups)
- [Discord — AutoMod](https://support.discord.com/hc/en-us/articles/4421269296535-AutoMod-FAQ)

## Nota metodológica

Este documento compara funções descritas publicamente e o estado documentado do GM Core na data da
revisão. Não representa benchmark de latência, disponibilidade ou capacidade máxima. Recursos dos
concorrentes podem depender de plano pago, configuração específica ou mudanças posteriores.
