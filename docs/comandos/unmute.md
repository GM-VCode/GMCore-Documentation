# `/unmute`

Remove os silenciamentos de chat e voz controlados pelo GM Core.

## Uso e acesso

```text
/unmute member:@membro reason:<motivo>
```

Exige `UNMUTE`, autoridade do dono ou equipe técnica.

## Funcionamento

O bot remove o timeout nativo, desfaz o mute de voz quando aplicável e elimina o registro ativo no
MongoDB. Também registra o motivo da retirada e envia a ação à auditoria. O comando encerra
conjuntamente os efeitos de chat e call que estiverem sob controle do bot.

O membro deve estar acessível no servidor e o bot precisa possuir as permissões nativas necessárias
para restaurá-lo.
