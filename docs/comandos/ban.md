# `/ban`

Bane uma conta pelo ID, inclusive quando ela já saiu do servidor.

## Uso e acesso

```text
/ban member:<ID> reason:<motivo>
```

Exige `BAN`, autoridade do dono ou equipe técnica. O motivo e um ID numérico válido são
obrigatórios.

## Funcionamento

O bot busca a conta pelo ID, valida se o alvo é protegido, executa o banimento e registra executor,
solicitante, alvo e motivo no histórico e no canal de auditoria correspondente.

## Recusas comuns

- alvo com proteção administrativa;
- ID inválido ou inexistente;
- ausência de `BAN`;
- cargo do bot sem permissão para banir;
- falha ou limite da API do Discord.

