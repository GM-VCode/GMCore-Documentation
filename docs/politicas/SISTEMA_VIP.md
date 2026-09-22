# Sistema VIP

## Finalidade

O sistema VIP administra benefícios temporários definidos pela comunidade: cargo global, call
particular, tag pessoal e acompanhantes. O GM Core não vende VIP, processa pagamento ou valida
comprovante.

## Funcionamento

A administração cadastra cargos, categorias e assinaturas com prazo. O titular pode administrar sua
única call, sua tag pessoal e acompanhantes dentro do limite recebido. O acompanhante precisa aceitar
o convite e não herda poderes administrativos nem o cargo VIP global.

Na expiração, o cargo é retirado e os recursos pessoais são removidos. A saída voluntária preserva a
assinatura válida para possível restauração; banimento encerra o benefício. Estruturas protegidas
apagadas fora do fluxo podem ser reconstruídas a partir do estado persistente.

## Dados e acesso

São mantidos servidor, cargos, categorias, titular, validade, recursos criados, acompanhantes e eventos
funcionais. A administração exige autorização específica; administrador nativo não recebe acesso
comercial automaticamente. Eventos são enviados ao canal `VIP_LOG` e os eventos funcionais
persistentes expiram em 2 dias.

## Limites

Cada titular possui no máximo uma call e uma tag pessoal. Tags pessoais não recebem permissões
administrativas sensíveis. Preço, cobrança, reembolso e entrega de benefícios externos permanecem sob
responsabilidade exclusiva da comunidade.
