# Projeto XY
Projeto sobre novo sistema em nuvem para a XY Brasil

## Objetivo
O Objetivo deste documento é facilitar a tomada de decisão sobre a implantação de um sistema em núvem para o novo sistema de gestão integrada para a empresa XY Brasil.

## On-Premisses VS SaaS
O uso de sistemas on-premisses é a forma mais tradicional de trabalhar com sistemas de gestão, já que o software acaba estando integrando ao patrimônio da empresa, quando um bug ou problema aparece muitas vezes a equipe sabe em qual linha de código está o erro, por ser tudo criando "em casa".
Com o crescimento das compras on-line o mercado logistico tem um papel fundamental e indispensável na entrega dos produtos físicos. Mas conforme o mercado avança, os outros players tem setado a barra cada vez mais alto, a própria complexidade das operações tem aumentado, conforme a cada dia que passa uma nova solução disruptiva é adicionada, criando um cenário onde quem não escala é deixado para trás.
Escalar a solução usando sistemas on-premisses é possível, mas o tamanho e nível de especialização da equipe seria tão alto que poderia tirar o foco da empresa, que é a gestão das operações logisticas e não cuidar de data-centers e criar algoritmos computacionais.
Com soluções SaaS é possível ampliar o produtividade da equipe de TI da empresa efetuar novas contratações, e sem precisar aumentar os custos com  Hardware e Licenças, na verdade existem uma grande chance dos custos baixarem ou pelo menos se estabilizarem sem impactar o crescimento da empresa.
Quando se trata de segurança o SaaS apresenta uma vantagem muita grande, uma delas é que mesmo em caso de ataque a equipe de segurança do fornecedor, consegue isolar o problema em um determinado cluster e manter outro datacenter funcionando como se nada tivesse acontecido. Outra grande vantagem é que em casos extremos as empresas SaaS se responsabilizam por possíveis danos e perdas, já __quando acontece algum incidente com um sistema _in-house_ empresa acaba levando todo prejuizo financeiro e jurídico sozinha__.

## Tatica de implantação
Como a empresa já tem vários sistemas rodando on-premisses a primeira opção seria buscar uma solução que já englobasse todos os sistemas em um só, a segunda opção seria um sistema que faz a maior parte das operações sendo necessário adicionar algumas customizações menores e a terceira opção seria a integração de vários sistemas SaaS, por exemplo, o setor de vendas vai usar o  ECM Fluig juntamente com o SugarCRM(SaaS) enquanto a equipe de Marketing vai usar uma solução SalesForce para as campanhas B2B e SharpSping para as campanhas B2C, nada impede que a equipe de TI trabalhe com maior foco no tratamento de dados relevantes e alimente em fluxo contínuo [chartio.com](chartio.com) para que os gestores da empresa possam ver os dados mais relevantes em um só lugar.
__Assim temos:__
* Tatica #1: SaaS Monolítico
* Tatica #2: SaaS com extensões
* Tatica #3: Vários sistemas SaaS inteligados

## Processo de implantação
### Análise de cenário
É muito difícil que a empresa esteja 100% com sistemas On-promisses, possivelemte boa parte da documentação dessa empresa já esteja no Google Docs, por exemplo. Outros pontos a se analisar são:
* ROI: É preciso analisar qual fornecedor vai entregar as features que a empresa usa no SLA que a empresa precisa, levando em consideração as vantagens de segurança que o SaaS de uma empresa conceituada traz.
* Cultura da empresa: nenhuma empresa fica grande sem desenvolver uma cultura, é necessário analisar e calcular quanto tempo levaria para os times absorverem novas ferramentas sem gerar buzz negativo, tourn-over desnecessário e medo de ser substituido pelos novos sistemas.
* Estimativa de tempo de implantação: Considerando motivos humanos (treinamento, cultura) e processuais (Levantamento de dados, migração do TI, jurídico).

### Migração Setorizada
Ainda que a empresa tenha encontrado um SaaS monolitico que vai cobrir todas as suas necessidades ou irá usar vários serviços integrados, a forma mais eficiente e menos dolorosa é realizar a migração seria setor-por-setor, cada um dos sistemas on-promisses para SaaS, migrando primeiro os sistemas periféricos e finalizando com a migração dos sistemas core, assim diminuido possíveis impáctos negativos ao funcionamento da empresa.

#### Migração de sistemas-periféricos
Sistemas perifericos são sistemas que não vão impactar diretamente na função principal da empresa durante a sua migração.
Vamos supor que a empresa use um _sisteminha_ que o pessoal do TI desenvolveu há muito tempo usando ASP e VB para cuidar do processo de recrutamento e seleção, isso pode ser subistituido pelo [https://dynamics.microsoft.com/pt-br/](MS Dynamics 365)

#### Migração de sistemas-core
Sistemas _core_ são sistemas que impactam diretamente no dia-a-dia da empresa.
Se o sistema que recebe as solicitações de transporte falha a empresa para, então esses sistemas seriam migrados por último.

### Treinamentos
Os treinamentos são parte fundamental da implantação do sistema, deve ficar claro que o sistema irá facilitar o trabalho do funcinário e não subistituilo. O desejo da empresa é crescer com a equipe e que os novos sistemas e metodologias poderão viabilizar formas mais confortáveis de se trabalhar, incluindo horários flexíveis, trabalho remoto.
Os gestores poderão melhorar a performance de seus setores assim melhorando os seus resultados e relatórios sem perder a hora da janta.
Se as pessoas virem o projeto como uma forma de fazer cortes na folha de pagamentos, a resistência pode retardar ou até inviabilizar toda a implantação do sistema o que aumenta o custo de implantação.
Treinamentos em empresas grandes são custosos porque param os funcionários de suas atividades por horas e as vezes por dias.
Todo setor tem aquele usuário que é mais familiarizado com a tecnologia e que entende as atividades do dia-a-dia do setor, mas conversa bem com a equipe de TI, esses seriam os usuários _focal-point_.
Ao invés de treinar a empresa inteira é melhor designar usuários _focal-point_ em cada setor, porque eles aprendem mais rápido e já estão habituados a auxiliar os seus colegas.

#### Treinamento da equipe de TI
A equipe de TI deve ser treinada para usar os novos sistemas e poder treinar e dar suporte para os _focal-points_ de cada setor. Dessa forma não consumindo as horas do cunsultor técnico da fornecedora, uma vez que sua hora/cunsultoria costuma ter valor elevado.

#### Treinamento dos usuários focal-point
Uma vez treinada, a equipe de TI deve treinar os usuários _focal-point_.
Ao invés de gastar 3 dias no autitório ou sala de reunião da empresa, com coffee-break, pausa para dúvidas. Pode-se investir 4 horas fazendo uma boa apresentação para o _focal-point_ do setor, é uma economia imensa para a empresa.

### Monitoria e Analytics
Uma vez implantado o sistema uma das tarefas da equipe de TI é monitorar e gerar relatórios sobre a performance do sistema.

## Atividades e rotinas
* __Weekly Meeting__: Uma reunião rápida de até 30 minutos no inicio da semana para revisão das tarefas do semana anterior e objetivação de metas da semana.
* __Daily Meetings__: Uma reunião rápida de até 30 minutos no início do dia para revisão das tarefas do dia anterior e objetivação de metas do dia, verificando sempre se não há um desvio desnecessário das metas objetivadas na _Weelky Meeting_
* __Rotina__:
  * Verificação e levantamento de warnings do sistema;
  * Check dos chamados dos usuários _Focal Point_;
  * Follow-up das respostas do suporte do fornecedor;
  * Investigação de novas práticas, melhorias e fornecedores;
  * fechamento de turno usando o documento padrão para report do dia.
 
## Métricas
### Cumprimento de SLA
* Verificar quanto tempo o fornecedor leva para adicionar as features, solucionar bugs e responder dúvidas
* Verificar o nível de entrega de seviço

### Resoluções em primeira chamada
* Manter um controle interno de quantas chamadas são resolvidas na primeira chamada de acordo com o SLA acertado.

### Tempo médio para atender
* Estar atento se em média o fornecedor atende em tempos condizentes com o SLA de cada chamado.

### Uptime
* Uptime de suporte: Tempo que o suporte leva para respondes às urgências.
* Uptime de infra: Tempo que o sistema funciona sem dar problemas.

### Tempo médio fora do ar
* Quando ocorre algum problema no sistema, em quanto tempo ele volta a operar integralmente.

### Tempo de resposta
* Tempo de resposta dos endpoints(REST/SOAP) e dos Scripts, observando o cumprimento de SLA.

### Tempo médio de atendimento
* Tempo que o suporte leva para chegar a solução em cada etapa do atendimento.

### Porcentagem de entregas com atraso
* Qual é a proporção dos atrasos do fornecedor e da equipe interna com as operações que rodam em SaaS.

### Comparação de dados
* Comparar todos os resultados da métricas SaaS com os resultados das métricas dos sistemas On-Premisses para fazer uma análise constante da viabilidade e ROI

## Conclusão
A menos que a empresa tenha a necessidade de poder colocar fogo no datacenter a qualquer momento para apagar os dados e torrar um bom dinheiro, SaaS é certamente a opção mais viável para empresas que querem crescer.
