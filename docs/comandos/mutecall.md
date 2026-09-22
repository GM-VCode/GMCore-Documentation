# `/mutecall`

Silencia temporariamente o microfone de um membro nos canais de voz.

## Uso e acesso

```text
/mutecall member:@membro reason:<motivo> time:<minutos>
```

Exige `MUTECALL`, autoridade do dono ou equipe técnica. O tempo precisa ser maior que zero.

## Funcionamento

- Se o membro já estiver em voz, o silenciamento é aplicado imediatamente.
- Se estiver fora de voz, o registro permanece ativo e o bot aplica quando ele entrar.
- O vencimento é salvo no MongoDB e verificado periodicamente pelo serviço de mutes.
- Ao terminar, o bot remove o efeito e encerra o registro ativo.

O SQLite é usado apenas pelos comandos `$` de contingência; o slash command opera pela persistência
principal no MongoDB.

Administradores protegidos não podem ser silenciados. Motivo, membro e duração são obrigatórios.
