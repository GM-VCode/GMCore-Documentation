# `/unban`

Revoga o banimento de uma conta pelo ID.

## Uso e acesso

```text
/unban user_id:<ID> reason:<motivo>
```

Exige `BAN`, autoridade do dono ou equipe técnica. ID e motivo são obrigatórios.

## Funcionamento

O bot resolve a conta pelo ID, remove o banimento no servidor, envia a confirmação e registra a
ação no histórico e na auditoria de banimentos.

O comando é recusado quando a conta não existe, não está banida, o solicitante não possui acesso
ou o bot não consegue administrar banimentos.

