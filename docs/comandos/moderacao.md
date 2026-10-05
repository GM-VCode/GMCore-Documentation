# `/moderacao`

Centraliza as ferramentas administrativas de uso diário.

## Uso

```text
/moderacao painel:<opção>
```

## Acesso

O dono, um Administrador nativo, o co-dono com `PROPRIETARIO`, a equipe técnica, quem possui
`MODERATION` ou a capacidade unitária da opção podem abrir o painel correspondente, desde que o
plano inclua a ferramenta.

## Opções

| Opção | Funcionamento | Capacidade unitária |
|---|---|---|
| Auditoria persistente | Filtra registros por origem, ação, período e ID | `CONSULTA` |
| Consultar histórico | Separa punições recebidas das ações aplicadas | `CONSULTA` |
| Minhas notificações | Preferências privadas de alertas por servidor | `CONSULTA` |
| Gerador de embeds | Criação, modelos, versões e publicação | `EMBED_MANAGE` |
| Limpar mensagens | Exclusão controlada de mensagens recentes ou antigas | `CLEAN_MESSAGES` |
| Consulta XP Staff | Busca por ID e mostra XP e horas válidas nas últimas 24 horas e 7 dias | `STAFF_XP_QUERY` |

## Gerador de embeds

A entrada apresenta três ações:

- **Criar:** começa um rascunho visual;
- **Editar:** abre por chave do modelo, ID ou link de publicação registrada;
- **Lista:** mostra os modelos e IDs salvos do servidor.

O editor configura mensagem comum, título, descrição, aparência, autor, rodapé, até 25 campos e
botões de link. Também oferece prévia, cópia, versões, arquivamento e publicação por ID do canal.

O formato V1 está disponível no Essencial e Pro; o V2, no Premium e Pro. Os limites de modelos
salvos e publicados são 15 no Essencial e 25 no Premium; o Pro oferece capacidade ampliada,
sujeita a uso responsável e suporte caso seja necessário ampliar. São aceitos até
cinco botões de link, ou quatro
quando existe um botão de anexo. Menções ficam desativadas na publicação. O bot só atualiza
mensagens criadas e registradas pelo próprio GM Core.

Os painéis administrativos usam containers integrados. A prévia e as mensagens publicadas pelo
Gerador de Embeds continuam como embeds clássicos para preservar o resultado configurado.

## Auditoria e histórico

A consulta de auditoria também inclui encerramentos recentes de tickets. O histórico é apoio para
decisão humana e não produz pontuação automática do membro.
