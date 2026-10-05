# `/help`

Abre a central privada de ajuda do GM Core dentro do Discord.

## Uso e acesso

```text
/help
```

Membros de servidores com plano ativo podem executar. Mesmo o Gratuito precisa ser ativado pela
equipe GM. Sem plano, a equipe comercial pode abrir a ajuda para acessar o Setup. A resposta é
privada e somente o solicitante pode usar seus componentes.

## Funcionamento

1. O bot apresenta uma lista com os comandos públicos atuais.
2. O usuário escolhe um comando.
3. O container passa a explicar acesso, funcionamento, limites e boas práticas.
4. **Anterior** e **Próxima** navegam pelas páginas daquele comando.
5. **Setup** apresenta o estado do bot e as opções disponíveis ao solicitante.

O catálogo cobre as centrais `/proprietario` e `/moderacao`, o módulo independente
`/ticket`, as punições, `/config`, `/vip` e `/xp`. Dentro da central do proprietário, a ajuda
explica separadamente contas, palavras, Anti-Link, Anti-Spam, Anti-Nuke e Bot-Moderação.

As páginas de segurança seguem o estado real do projeto: todas as proteções começam desativadas,
cada módulo informa seu acesso e o Anti-Nuke exige plano Essencial ou superior e autoridade
compatível, inclusive co-dono delegado.

O botão **Setup** apresenta uma visão segura aos membros e controles próprios às equipes autorizadas.

## Observações

- O painel expira após dez minutos.
- Outros usuários não conseguem controlar a sessão.
- Os comandos `$` aparecem apenas como contingência; não substituem os slash commands.
- A lista e os botões de navegação ficam integrados ao mesmo container.
