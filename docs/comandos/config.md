# `/config`

Administra a ACL interna do GM Core para um usuário ou cargo do servidor.

## Uso

```text
/config alvo:@usuário-ou-cargo
```

## Acesso

Exige uma destas condições:

- ser o dono do servidor;
- possuir `CONFIG_EDIT` diretamente como usuário;
- integrar a equipe técnica oficial.

`CONFIG_EDIT` não é herdada por cargo. Isso impede que a autoridade de redistribuir permissões seja
ampliada indiretamente.

## Funcionamento

1. Selecione o alvo no próprio comando.
2. Escolha uma capacidade no seletor.
3. Use **Adicionar** ou **Remover**.
4. Use **Lista** para consultar as concessões do servidor.
5. **Remover Tudo** revoga todas as capacidades internas do alvo.

O painel é privado, pertence ao solicitante e atualiza a mesma mensagem durante a sessão.
O seletor, os botões e a lista paginada ficam integrados ao container do painel.

## Capacidades amplas e unitárias

- `PROPRIETARIO`: herda as opções estruturais declaradas para a central do dono.
- `MODERATION`: herda as ferramentas declaradas para a central de moderação.
- `TICKET_MANAGE`: controla exclusivamente o módulo de tickets.
- Capacidades como `BAN`, `KICK`, `CONSULTA`, `EMBED_MANAGE` e `VIP_MANAGE` concedem somente a
  operação correspondente.

As capacidades internas não removem validações de hierarquia nem criam permissões nativas no
Discord.
