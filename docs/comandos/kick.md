# `/kick`

Expulsa um membro sem impedir que ele volte por um novo convite.

## Uso e acesso

```text
/kick member:<ID-ou-menção> reason:<motivo>
```

Exige `KICK`, autoridade do dono ou equipe técnica. O bot aceita ID ou menção no campo `member`.

## Funcionamento

O alvo precisa estar no servidor. O comando valida o motivo, a proteção administrativa e a
hierarquia antes de expulsar. Em caso de sucesso, registra solicitante, executor, alvo e motivo no
histórico e na auditoria.

O bot recusa administradores protegidos, alvos inexistentes e situações em que sua própria
permissão ou posição de cargo é insuficiente.

