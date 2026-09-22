# `/help`

Abre a central privada de ajuda do GM Core dentro do Discord.

## Uso e acesso

```text
/help
```

Todos os membros podem executar. A resposta é efêmera e somente o solicitante pode usar seus
componentes.

## Funcionamento

1. O bot apresenta uma lista com os comandos públicos atuais.
2. O usuário escolhe um comando.
3. O container passa a explicar acesso, funcionamento, limites e boas práticas.
4. **Anterior** e **Próxima** navegam pelas páginas daquele comando.
5. **Setup** abre o diagnóstico de conexão e saúde do bot.

O catálogo cobre as centrais `/proprietario` e `/moderacao`, o módulo independente
`/ticket suporte`, as punições, `/config` e `/vip`. Dentro da central do proprietário, a ajuda
explica separadamente contas, palavras, Anti-Link, Anti-Spam, Anti-Nuke e Bot-Moderação.

As páginas de segurança seguem o estado real do projeto: todas as proteções começam desativadas,
cada módulo informa sua capacidade ACL e o Anti-Nuke identifica que somente o dono real pode
configurá-lo.

O botão **Setup** aparece para todos. Membros comuns recebem a visão segura; a equipe técnica recebe
os controles adicionais já protegidos pelo sistema.

## Observações

- O painel expira após dez minutos.
- Outros usuários não conseguem controlar a sessão.
- Os comandos `$` aparecem apenas como contingência; não substituem os slash commands.
- A lista e os botões de navegação ficam integrados ao mesmo container.
