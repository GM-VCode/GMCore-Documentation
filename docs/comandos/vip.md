# `/vip`

Abre o painel pessoal de uma assinatura VIP vigente.

## Uso e acesso

```text
/vip
```

O titular precisa possuir um VIP ativo. Administradores configuram cargos, categorias e
assinaturas pela opção **Administração VIP** de `/proprietario`.

## Recursos do titular

- criar uma call pessoal e editar nome ou limite;
- criar e editar tags até o limite definido para o cargo VIP;
- adicionar ou remover acesso aos recursos;
- consultar a lista de pessoas autorizadas;
- atualizar o painel e visualizar a validade.

Existe somente uma call pessoal por assinatura. Calls vazias são tratadas pelo agendador de limpeza
e o sistema acompanha alterações ou exclusões de cargos e canais.

## Acompanhantes

Acompanhante é um vínculo de benefício, não uma segunda assinatura. Ele não recebe `/vip`, call
própria, tags próprias ou poderes do titular. Seu painel permite apenas encerrar o próprio vínculo.

Expirações são verificadas periodicamente pelo bot e os recursos seguem a política da assinatura
administrada pelo servidor.

Os botões e as listas dos painéis administrativo, titular e acompanhante ficam integrados aos
respectivos containers.
