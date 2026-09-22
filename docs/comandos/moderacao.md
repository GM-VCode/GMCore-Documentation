# `/moderacao`

Centraliza as ferramentas administrativas de uso diário.

## Uso

```text
/moderacao painel:<opção>
```

## Acesso

O dono, um Administrador nativo, a equipe técnica, quem possui `MODERATION` ou a capacidade
unitária da opção podem abrir o painel correspondente.

## Opções

| Opção | Funcionamento | Capacidade unitária |
|---|---|---|
| Auditoria persistente | Filtra registros por origem, ação, período e ID | `CONSULTA` |
| Consultar histórico | Separa punições recebidas das ações aplicadas | `CONSULTA` |
| Minhas notificações | Preferências privadas de alertas por servidor | `CONSULTA` |
| Gerador de embeds | Criação, modelos, versões e publicação | `EMBED_MANAGE` |
| Limpar mensagens | Exclusão controlada de mensagens recentes ou antigas | `CLEAN_MESSAGES` |

## Gerador de embeds

A entrada apresenta quatro ações:

- **Criar:** começa um rascunho visual;
- **Editar:** abre por chave do modelo, ID ou link de publicação registrada;
- **Modelos:** lista os modelos ativos do servidor;
- **Lista:** mostra as publicações registradas que ainda existem.

O editor configura mensagem comum, título, descrição, aparência, autor, rodapé, até 25 campos e
botões de link. Também oferece prévia, cópia, versões, arquivamento e publicação por ID do canal.

Cada servidor pode manter até 25 modelos ativos. São aceitos até cinco botões de link, ou quatro
quando existe um botão de anexo. Menções ficam desativadas na publicação. O bot só atualiza
mensagens criadas e registradas pelo próprio GM Core.

Os painéis administrativos usam containers integrados. A prévia e as mensagens publicadas pelo
Gerador de Embeds continuam como embeds clássicos para preservar o resultado configurado.

## Auditoria e histórico

A consulta de auditoria também inclui encerramentos recentes de tickets. O histórico é apoio para
decisão humana e não produz pontuação automática do membro.
