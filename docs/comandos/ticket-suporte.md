# `/ticket`

Configura os tickets de suporte e, a partir do Premium, os de sorteio.

## Uso e acesso

```text
/ticket painel: Ticket de Suporte
/ticket painel: Ticket de Sorteio
```

O suporte exige plano Essencial ou superior; o sorteio, Premium ou Pro. O painel exige ser dono
do servidor, co-dono com `PROPRIETARIO`, integrar a equipe técnica ou possuir `TICKET_MANAGE`.
Administrador nativo, sozinho, não recebe esse acesso.

## Configuração

O painel privado permite definir:

- cargo responsável pelo suporte;
- canal público onde o painel será publicado;
- título, descrição, cor, imagem, thumbnail e rodapé da apresentação pública;
- estado ativo ou inativo do atendimento.

No Premium e Pro, configure `TICKET_LOG` para receber o relatório do atendimento.

## Fluxo do usuário

1. O usuário pressiona **Abrir Ticket** no painel público.
2. O bot cria um tópico privado para autor, suporte e bot.
3. Um integrante da equipe usa **Pegar ticket**.
4. O atendente conversa, adiciona pessoas ou cria uma call privada sob demanda.
5. O atendente, Administrador nativo ou `TICKET_MANAGE` finaliza.
6. No Premium e Pro, um relatório HTML é enviado ao `TICKET_LOG`; no Essencial, o atendimento
   é encerrado sem esse relatório.
7. O tópico é arquivado e o botão de exclusão é liberado.

Os controles públicos e privados ficam dentro de containers. Os mesmos identificadores
persistentes continuam registrados para funcionar depois de reiniciar o bot.

## Regras

- Um usuário mantém apenas um Ticket de Suporte aberto por vez.
- Existe somente um atendente responsável e uma call por ticket.
- A call nasce com limite de duas pessoas e pode ser ajustada pela equipe.
- O autor comum não pode finalizar o próprio ticket.
- Participantes de texto, voz ou inclusão manual aparecem no registro.
- Quando o relatório estiver incluído no plano, o canal `TICKET_LOG` deve estar disponível.

## Sorteios

No Premium e Pro, a equipe pode publicar um painel de participação, configurar prazo e canais,
e consultar o resultado. Cada membro humano participa uma vez por campanha.
