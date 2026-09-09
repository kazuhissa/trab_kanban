Desenvolvimento do quadro Kanban feito no Figma ( Link abaixo )
https://www.figma.com/design/rzPAc2XXawoSqQC82vAdoP/Guia-de-Estilo-e-Prototipos?node-id=0-1&t=S5ACv2IsX8eerj4K-1


Sistema de suporte técnico - UmuprevTech 

O UmuprevTech é um sistema interno de suporte técnico utilizado pelos funcionários da empresa para registrar solicitações e problemas relacionados à área de Tecnologia da Informação (TI). A equipe de TI é responsável por receber, analisar, priorizar e solucionar os chamados realizados pelos funcionários. 

Quem usa o sistema? 

Funcionários internos da empresa, que abrem os chamados; 

Equipe de TI, responsável por analisar e resolver as solicitações. 

Quem são os clientes/usuários? 

Os próprios funcionários da UmuprevTech que necessitam de suporte técnico para realizar suas atividades de trabalho. 

Que tipos de demandas chegam para a equipe de TI? 

Computador ou notebook com problemas; 

Problemas de acesso à internet ou à rede; 

Impressoras que não funcionam; 

Instalação ou configuração de softwares; 

Problemas de login ou senha; 

Solicitação de criação ou alteração de acessos; 

Problemas em sistemas internos; 

Manutenção ou configuração de equipamentos. 

Onde o trabalho começa? 

O trabalho começa quando um funcionário interno abre um chamado no sistema, descrevendo o problema ou a necessidade de suporte. A equipe de TI recebe o chamado, realiza a triagem e define a prioridade e os próximos passos para atendimento. 

Quando podemos considerar que algo foi entregue? 

O chamado é considerado entregue quando a equipe de TI resolve o problema ou atende à solicitação, realiza as validações necessárias e registra a solução no sistema. O chamado então é encerrado e o funcionário é informado sobre a conclusão. 

Fluxo do atendimento 

Funcionário abre o chamado 

↓ 

Chamado recebido 

↓ 

Triagem / Priorização 

↓ 

Pronto para atendimento 

↓ 

Em atendimento 

↓ 

Testes / Validação 

↓ 

Resolvido 

↓ 

Chamado encerrado 

Definir as políticas explícitas 

As políticas são as regras que a equipe de TI vai seguir para movimentar os chamados no Kanban. Elas estabelecem critérios para entrada, seleção, movimentação, bloqueios, urgências e entrega. 

Política de entrada 

Um chamado só entra no fluxo quando o funcionário informar as informações necessárias para identificar o problema, como descrição da solicitação, setor e equipamento ou sistema afetado. 

Política de prioridade 

A equipe de TI analisa cada chamado e define sua prioridade de acordo com o impacto do problema. 

Alta: problema impede o funcionário de trabalhar ou afeta vários funcionários; 

Média: problema prejudica o trabalho, mas existe uma alternativa temporária; 

Baixa: solicitação simples ou que não impede o trabalho. 

Política de urgência 

Chamados classificados como Alta prioridade terão preferência no atendimento quando impedirem totalmente o trabalho de um funcionário ou afetarem vários funcionários. 

A equipe deverá avaliar a urgência antes de puxar novos chamados e, quando necessário, reorganizar a ordem dos atendimentos para reduzir o impacto causado pelo problema. 

Política de puxada 

Um novo chamado só pode ser puxado para Em atendimento quando houver espaço dentro do limite de WIP dessa etapa. 

A equipe deve evitar iniciar novos chamados enquanto o limite de WIP estiver atingido, priorizando a conclusão dos trabalhos que já estão em andamento. 

Política de atendimento 

A equipe deve priorizar a conclusão dos chamados que já estão em atendimento antes de iniciar novos chamados. 

Quando existir capacidade disponível, a equipe pode puxar um novo chamado de acordo com sua prioridade e com as regras definidas para o fluxo. 

Política de bloqueio 

Quando um chamado depender de outra pessoa, setor, fornecedor ou recurso externo, ele deve ser marcado como Bloqueado, informando o motivo. 

O chamado bloqueado permanece visível no quadro para que a equipe acompanhe sua situação e possa agir quando a dependência for resolvida. 

Política para chamados bloqueados 

Quando um chamado estiver bloqueado por uma dependência externa e não estiver consumindo trabalho ativo da equipe de TI, ele poderá ser retirado temporariamente da capacidade de trabalho ativo da etapa, sem deixar de ser visível no Kanban. 

Dessa forma, a equipe consegue puxar outro chamado e continuar trabalhando enquanto o item bloqueado aguarda a resolução da dependência. 

Política de validação 

Depois de solucionar o problema, a equipe realiza os testes necessários para verificar se a solução funcionou. 

Quando necessário, o funcionário que abriu o chamado também poderá validar se o problema foi solucionado. 

Política de entrega 

O chamado só pode ser considerado Resolvido/Encerrado quando o problema estiver solucionado, a solução estiver registrada e o funcionário tiver sido informado. 

Registro da Simulação — UmuprevTech 

Problema observado: 

Acúmulo excessivo de cartões na coluna Em Atendimento, causado principalmente por chamados que ficaram bloqueados aguardando uma dependência externa, como liberação de acesso, fornecedor ou outro setor. 

Evidência: 

Durante as rodadas da simulação, alguns chamados permaneceram parados por dependerem de terceiros. Como o limite de WIP da etapa de atendimento havia sido atingido, a equipe ficou impedida de puxar novas demandas, mesmo existindo chamados de menor complexidade que poderiam ser resolvidos rapidamente. Isso demonstrou que o bloqueio de um chamado estava prejudicando o fluxo dos demais atendimentos. 

Hipótese: 

Se a equipe criar uma identificação específica para chamados Bloqueados por Dependência Externa, será possível diferenciar o trabalho ativo daquele que está aguardando terceiros, permitindo que a equipe continue atendendo outras solicitações. 

Experimento: 

Foi criada uma identificação visual para chamados bloqueados e estabelecida uma regra para que chamados aguardando dependências externas sejam retirados temporariamente da capacidade de trabalho ativo da equipe, permanecendo visíveis no quadro. 

O objetivo foi evitar que um chamado parado por uma dependência externa ocupasse uma vaga de trabalho que poderia ser utilizada para atender outra solicitação. 

Resultado: 

O comportamento do fluxo melhorou, pois a equipe conseguiu continuar atendendo chamados que não possuíam dependências externas enquanto os chamados bloqueados aguardavam a resolução de suas dependências. 

A alteração também reduziu o acúmulo na etapa de atendimento e permitiu que o sistema mantivesse o fluxo de chamados mesmo quando existiam impedimentos externos. 

Próximo passo: 

Implementar uma regra no sistema web para que o analista possa marcar um chamado como Bloqueado por Dependência Externa, registrando o motivo e notificando automaticamente o responsável pelo desbloqueio. 

Além disso, a equipe deverá continuar observando o comportamento do fluxo para verificar se os limites de WIP definidos continuam adequados. 

 
