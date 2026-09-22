# `/ticket suporte`

Configura, publica e administra o primeiro tipo de ticket do GM Core.

## Uso e acesso

```text
/ticket suporte
```

O painel de configuração exige ser dono do servidor, integrar a equipe técnica ou possuir
`TICKET_MANAGE`. Administrador nativo, sozinho, não abre este comando.

## Configuração

O painel privado permite definir:

- cargo responsável pelo suporte;
- canal público onde o painel será publicado;
- título, descrição, cor, imagem, thumbnail e rodapé da apresentação pública;
- estado ativo ou inativo do atendimento.

Antes de operar, abra `/proprietario painel: Configuração do servidor` e use **Canais de
auditoria** para garantir o canal `TICKET_LOG`.

## Fluxo do usuário

1. O usuário pressiona **Abrir Ticket** no painel público.
2. O bot cria um tópico privado para autor, suporte e bot.
3. Um integrante da equipe usa **Pegar ticket**.
4. O atendente conversa, adiciona pessoas ou cria uma call privada sob demanda.
5. O atendente, Administrador nativo ou `TICKET_MANAGE` finaliza.
6. O transcript HTML é enviado ao `TICKET_LOG`.
7. O tópico é arquivado e o botão de exclusão é liberado.

Os controles públicos e privados ficam dentro de containers. Os mesmos identificadores
persistentes continuam registrados para funcionar depois de reiniciar o bot.

## Regras

- Um usuário mantém apenas um Ticket de Suporte aberto por vez.
- Existe somente um atendente responsável e uma call por ticket.
- A call nasce com limite de duas pessoas e pode ser ajustada pela equipe.
- O autor comum não pode finalizar o próprio ticket.
- Participantes de texto, voz ou inclusão manual aparecem no registro.
- Sem `TICKET_LOG`, o encerramento é recusado para evitar perda do transcript.
- Estado operacional e resumo diário mínimo expiram do MongoDB após sete dias.
