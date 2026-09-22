# `/mutechat`

Impede temporariamente um membro de interagir no chat do servidor.

## Uso e acesso

```text
/mutechat member:@membro reason:<motivo> time:<5s|10m|2h|28d>
```

Exige `MUTECHAT`, autoridade do dono ou equipe técnica. A duração aceita `s` para segundos, `m`
para minutos, `h` para horas e `d` para dias. O mínimo é `5s` e o máximo é `28d`.

## Funcionamento

O bot aplica o timeout nativo ao membro inteiro. Isso bloqueia sua comunicação em todos os canais
do servidor, inclusive os criados depois da punição, sem criar sobrescritas individuais. Motivo,
duração exata e vencimento ficam no MongoDB.

O recurso funciona em qualquer servidor, inclusive sem o modo Comunidade. O bot precisa da
permissão nativa **Moderar membros**, e o cargo dele deve estar acima do cargo do membro atingido.

Se o membro sair e retornar antes do vencimento, o listener de entrada consulta o registro ativo e
reaplica imediatamente o tempo restante. O ciclo periódico de mutes funciona como redundância. O
Discord remove o timeout no vencimento e o bot encerra o registro e o histórico operacional.

O comando recusa administradores protegidos, duração inválida, ausência de motivo, falta de acesso
ou hierarquia insuficiente do bot.
