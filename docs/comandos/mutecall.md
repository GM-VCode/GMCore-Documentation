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
- O vencimento é acompanhado pelo bot para retirar o silenciamento no prazo.
- Ao terminar, o bot remove o efeito e encerra o registro ativo.

Em indisponibilidade do serviço principal, os comandos de contingência oferecem apenas ações
essenciais; eles não substituem o funcionamento completo dos comandos do Discord.

Administradores protegidos não podem ser silenciados. Motivo, membro e duração são obrigatórios.
