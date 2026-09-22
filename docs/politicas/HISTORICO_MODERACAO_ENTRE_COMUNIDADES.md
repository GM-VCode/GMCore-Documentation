# Política do Histórico de Moderação entre Comunidades — GM Core

> **Versão:** 1.0  
> **Última revisão:** 22 de setembro de 2026
> **Estado:** em crescimento e desenvolvimento

O recurso já possui funcionamento básico e acesso restrito, mas continua evoluindo. Regras,
apresentação, cobertura entre comunidades e mecanismos de governança podem receber ajustes antes de
o sistema ser tratado como uma funcionalidade plenamente estabilizada.

## 1. Finalidade

O Histórico de Moderação entre Comunidades do GM Core auxilia equipes autorizadas a consultar
ocorrências administrativas anteriores relacionadas a uma conta do Discord.

Sua finalidade é oferecer contexto para decisões de segurança e moderação quando uma conta possui
registros em mais de uma comunidade que utiliza o GM Core.

O sistema não cria uma lista pública de usuários, não monitora conversas entre servidores e não
permite que membros comuns consultem os registros.

## 2. Como a consulta funciona

A conta é localizada pelo ID numérico disponibilizado pelo próprio Discord.

O responsável pela moderação copia o ID usando o recurso nativo da plataforma ou seleciona a conta
no comando correspondente. O GM Core utiliza esse identificador somente para localizar a ficha
correta.

```text
Discord
   ↓
Moderador autorizado seleciona a conta ou copia seu ID
   ↓
GM Core localiza a ficha correspondente
   ↓
O painel privado apresenta o histórico permitido
```

O sistema não realiza uma busca pública ou indiscriminada de usuários. A consulta depende de uma
ação intencional de uma pessoa autorizada.

## 3. Informações apresentadas

Para cada ocorrência, o painel pode apresentar:

- tipo da punição ou medida administrativa;
- motivo registrado;
- comunidade em que a ocorrência aconteceu;
- data da ocorrência;
- duração, quando aplicável.

A ficha também pode mostrar a quantidade de punições recebidas, medidas aplicadas e comunidades
representadas no histórico.

## 4. Informações que não são apresentadas

A consulta entre comunidades não revela:

- quem aplicou a punição;
- identidade de denunciantes ou testemunhas;
- mensagens privadas;
- conteúdo de conversas;
- anexos ou arquivos;
- endereço IP, localização ou informações externas ao Discord;
- tokens, credenciais ou dados de autenticação;
- logs gerais de auditoria da comunidade.

A informação usada para identificar diretamente a conta consultada é seu ID do Discord, acompanhado
do nome conhecido quando estiver disponível na própria plataforma.

## 5. Quem pode consultar

O histórico não pode ser acessado por membros comuns.

A consulta é permitida somente a pessoas autorizadas na comunidade em que o comando é executado,
como:

- proprietário do servidor;
- administrador ou moderador com permissão nativa compatível;
- usuário ou cargo autorizado pela capacidade interna `CONSULTA`;
- equipe técnica oficial, quando necessário para operação e suporte.

As permissões são verificadas antes da exibição. O painel é efêmero e fica visível somente para a
pessoa autorizada que realizou a consulta.

## 6. Separação da auditoria interna

O Histórico de Moderação entre Comunidades não é o mesmo sistema dos canais de auditoria internos.

Os logs gerais de uma comunidade permanecem vinculados ao respectivo servidor e não são entregues a
outras comunidades. O histórico compartilhado apresenta somente o resumo limitado das ocorrências
de moderação descrito nesta política.

Configurações, alterações de cargos, mensagens apagadas, movimentações em canais de voz, ações
internas da equipe e demais eventos administrativos não fazem parte da consulta entre comunidades.

## 7. Natureza informativa

Uma ocorrência externa serve somente como informação de apoio. Ela não gera punição automática e
não obriga outra comunidade a repetir a decisão original.

Cada equipe continua responsável por:

- analisar o contexto apresentado;
- considerar suas próprias regras;
- avaliar a atualidade e a gravidade do registro;
- decidir de forma humana e proporcional.

O GM Core não atribui pontuação de risco, não classifica automaticamente pessoas e não recomenda
banimentos automáticos com base no histórico.

## 8. Uso permitido

O sistema deve ser utilizado somente para:

- moderação e segurança da comunidade;
- prevenção de abuso recorrente;
- análise administrativa de ocorrências;
- continuidade das decisões da equipe de moderação;
- proteção dos membros da comunidade.

É proibido utilizar a consulta para perseguição, constrangimento, discriminação, exposição pública,
retaliação ou curiosidade sem finalidade administrativa.

## 9. Minimização e proteção

O GM Core apresenta somente as informações necessárias para compreender a ocorrência.

O sistema não mostra a identidade de quem puniu e não compartilha o conteúdo que originou a medida.
Isso reduz a exposição de moderadores, denunciantes, testemunhas e demais pessoas envolvidas.

O histórico fica restrito às interfaces protegidas do bot e não é disponibilizado como consulta
pública.

## 10. Limitações

O histórico representa medidas administrativas tomadas por comunidades independentes. Regras e
critérios podem variar entre servidores, e um motivo registrado pode não conter todo o contexto da
situação original.

Por isso:

- um registro não representa condenação judicial;
- a existência de uma punição não determina automaticamente uma nova punição;
- o histórico deve ser usado como apoio, e não como decisão automática;
- a decisão final pertence à equipe da comunidade que realizou a consulta.

## 11. Proteção de crianças e adolescentes

O sistema não deve ser usado para expor relatos sensíveis ou ampliar riscos envolvendo crianças e
adolescentes. Situações graves devem ser encaminhadas pelos mecanismos oficiais de denúncia do
Discord e, quando necessário, às autoridades ou serviços competentes.

O GM Core é uma ferramenta administrativa. Ele não substitui os mecanismos de segurança da
plataforma, serviços de emergência ou investigações oficiais.

## 12. Relação com o Discord

O GM Core utiliza o identificador e as permissões disponibilizados pelo Discord para executar a
consulta.

O uso do ID é limitado à identificação da conta e à localização do histórico correspondente. O
recurso não depende de dados externos à plataforma e não permite acesso público às fichas.

Caso solicitado pelo Discord, esta política demonstra:

- a finalidade administrativa e de segurança;
- o fluxo de autorização da consulta;
- as informações efetivamente apresentadas;
- a separação entre auditoria interna e histórico entre comunidades;
- a proteção da identidade de quem aplicou a punição;
- a ausência de punições automáticas;
- a impossibilidade de acesso por membros comuns.

## 13. Resumo

```text
Quem consulta:
somente moderação autorizada

Como a conta é localizada:
ID copiado ou conta selecionada pelo próprio Discord

O que aparece:
punição, motivo, comunidade, data e duração aplicável

O que não aparece:
quem puniu, conversas, mensagens privadas, anexos ou dados externos

O que o sistema faz:
fornece contexto administrativo

O que o sistema não faz:
não pune automaticamente e não disponibiliza o histórico ao público
```

## 14. Observação jurídica

Este documento descreve a finalidade e o funcionamento do recurso. Ele não constitui parecer
jurídico e não substitui a avaliação das normas aplicáveis ao serviço.
