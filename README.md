# Trabalho de Conclusão de Curso

Repositório para armazenar a produção relacionada ao meu trabalho de conclusão de
curso para o bacharelado em psicologia na PUCRS.

## Escolha do tema

Algumas ideias para tema de pesquisa.

### Educação, dinheiro e psicoterapia

Investigar como fatores socioeconômicos, como nível de escolaridade e renda, estão
relacionados com desfechos de uma intervenção psicoterápica.

[Dados abertos de um estudo sobre a eficácia de intervenção.](https://openpsychologydata.metajnl.com/articles/10.5334/jopd.35)

#### Estudos (possivelmente) relacionados

* [Web-based positive psychology interventions: A reexamination of effectiveness.](https://doi.org/10.1002/jclp.22328)
* [Predicting individual response to a web-based positive psychology intervention: A machine learning approach.](https://doi.org/10.1080/17439760.2023.2254743)
* [Predicting optimal interventions for clinical depression: Moderators of outcomes in a positive psychological intervention vs. cognitive-behavioral therapy.](https://doi.org/10.1016/j.genhosppsych.2019.07.004)
* [Meta-analysis: The effectiveness of youth psychotherapy interventions in low- and middle-income countries.](https://doi.org/10.1016/j.jaac.2022.12.005)
* [The effectiveness of a web-based positive psychology intervention in enhancing college students’ mental well-being.](https://doi.org/10.2224/sbp.10459)
* [The long and winding road to happiness: A randomized controlled trial and cost-effectiveness analysis of a positive psychology intervention for lonely people with health problems and a low socio-economic status.](https://doi.org/10.1186/s12955-020-01416-x)
* [Positive psychological interventions and information and communication technologies.](https://doi.org/10.4018/978-1-7998-3432-8.ch083)

### Psicoterapeuta também é gente

Investigar a relação entre estilo pessoal da psicoterapeuta e os defechos de uma
intervenção psicoterápica.

## Fichamento de artigos

### Predicting individual response to a web-based positive psychology intervention: a machine learning approach

#### Autores

Amanda C. Collins, George D. Price, Rosalind J. Woodworth e Nicholas C. Jacobson.

#### Ano

2023.

#### Problema

Intervenções em psicologia positiva mostram-se efetivas no tratamento de sintomas
depressivos e aumento da felicidade, mas nem todos pacientes respondem conforme o
esperado. É importante identificar indivíduos com menores chances de resposta a esse
tipo de intervenção para que possam ser encaminhados a outros tipos de tratamentos.

#### Objetivo

Investigar se características individuais seriam capazes de prever modificações nos
níveis de felicidade e de sintomas depressivos de uma pessoa após a participação em
uma intervenção de psicologia positiva on-line; investigar quais características do
indivíduo tem maior contribuição para previsão do desfecho.

#### Metodologia

##### Participantes

Participaram 295 cidadãos australianos recrutados através de anúncios em jornais, rádios,
televisão e artigos da Internet para participar de um estudo sobre felicidade.

##### Intervenção

Os participantes foram distribuídos aleatoriamente em 4 grupos: 3 grupos de intervenção
(gratidão, forças de caráter e três coisas boas) e um grupo de controle ativo (memórias de
antigas). Cada grupo recebeu um e-mail com um conjunto de instruções específicas:

- Gratidão: escrever uma carta agradecendo uma pessoa que teve influência positiva em
sua vida mas nunca foi agradecida.

- Forças de caráter: preencher um questionário para identificação das forças de caráter,
ler as descrições de cada uma delas e buscar aplicá-las ao longo da semana.

- Três coisas boas: anotar três coisas boas que aconteceram ao longo do dia e explicar
por que elas aconteceram.

- Memórias antigas: escrever memórias antigas ao final do dia.

##### Desfechos observados

Foram observados os níveis de felicidade e sintomas depressivos conforme avaliados pelos
instrumentos *Authentic happiness inventory* (AHI) e *Center for epidemiologic studies
depression scale* (CES-D) respectivamente.

##### Procedimentos

Os participantes completaram um questionário com informações demográficas e preencheram
escalas de felicidade e sintomas depressivos, formando a observação de base.  Eles então
passaram pela intervenção que teve duração de uma semana. Os níveis de felicidade e sintomas
depressivos dos participantes foram avaliados imediatamente, uma semana, um mês, três meses
e seis meses após o fim da intervenção.

##### Plano de análise de dados

Foram treinados modelos de machine learning do tipo *extreme gradient boosted tree*, um para
cada comparação entre dados de base e pós-teste e para cada uma das medidas (AHI e CES-D),
totalizando 10 modelos. Foi usada a abordagem *leave-one-out cross-validation* (70%/30%) para
avaliação do desempenho dos modelos. 

Empregaram também o procedimento de *Shapley additive explanations* (SHAP) para estimar a
contribuição de cada característica da entrada no desfecho previsto pelo modelo e elencaram
as 5 características mais releventes para a previsão.

##### Resultados

Os pesquisadores encontraram correlação moderada entre os dados reais e as previsões do
modelo para níveis de felicidade (r = 0.30) e sintomas depressivos (r = 0.39) avaliados
seis meses após o fim da intervenção. Em ambos os casos, características clínicas (avaliadas
pelo AHI e CES-D no pré-teste) tiveram maior contribuição para a previsão do desfecho.

##### Limitações

A amostra era pequena e consistia majoritariamente de pessoas com níveis não-clínicos de
depressão, o que limita a possibilidade de generalização dos modelos para populações clínicas.
Não foram examinados fatores importantes que podem ter contribuído para os resultados da
intervenção, como nível de engajamento dos participantes.


### Predicting therapy outcome in a digital mental health intervention for depression and anxiety: A machine learning approach

#### Autores

Silvan Hornstein, Valerie Forman-Hoffman, Albert Nazander, Kristian Ranta e Kevin Hilbert.

#### Ano

2021.

#### Problema

Embora a necessidade de tratamentos individualizados em saúde mental seja cada mais reconhecida,
ainda existem poucos trabalhos que avaliam a viabilidade do uso de algoritmos de *machine
learning* para fazer previsões sobre a resposta a intervenções a nível individual.


#### Objetivo

Avaliar o desempenho de algoritmos de *machine learning* na previsão dos resultados de uma
intervenção digital em saúde mental projetada para o tratamento de ansiedade e depressão.

#### Metodologia

##### Participantes

Foram coletados dados anônimos de 970 pessoas usuárias do *Meru Health Program* (as pessoas
consentiram com o uso dos dados anonimizados para realização de pesquisa ao ingressar no programa).

##### Intervenção

O *Meru Health Program* é um programa digital em saúde mental com foco em ansiedade e depressão
realizado via smartphone. A intervenção consiste na aplicação técnicas de TCC, psicoeducação,
exercícios de mindfulness e biofeedback ao longo de um período que varia entre 8 e 12 semanas.
Os participantes são acompanhados por psicoterapeutas clínicos licenciados que revisam engajamento
e resultados e mantém contato assíncrono frequente por meio de mensagens.

##### Desfechos observados

Os resultados da intervenção foram acompanhados com a aplicação dos instrumentos *Patient Health
Questionaire-9* (PHQ-9) e *General Anxiety Disorder Screener-7* (GAD-7) a cada duas semanas. O
principal desfecho de interesse foi uma variável binária de resposta/não resposta à intervenção,
definida como uma redução significativa nos sintomas de ansiedade ou depressão (redução de pelo
menos 5 pontos na PHQ-9 ou pelo menos 4 pontos na GAD-7).

##### Plano de análise de dados

Usando dados clínicos de uma primeira aplicação do PHQ-9, do GAD-7 bem como dados demográficos,
Foram treinados modelos de *machine learning* dos tipos: regressão logística, *support vector
machine*, *naive Bayes* e *random forest* (RF). A performance dos modelos foi avaliada usando a técnica
de *10-fold cross-validation* e o método de imputação de dados utilizado para cada modelo foi avaliado e
selecionado como parte do processo de *cross-validation*. O ajuste de hiper-parâmetros foi feito
usando o método de *exhaustive grid search*. O principal indicador de performance dos modelos na
fase de *cross-validation* foi a medida de *receiver operating characteristics area under curve*
(ROC AUC).

##### Resultados

Na etapa de *cross-validaiton* o algoritimo RF apresentou o melhor resultado (ROC AUC = 0.64) e
foi utilizado em uma rodada de teste contra um conjunto de 279 novas observações, obtendo uma
precisão não balanceada de 0.71 com ROC AUC de 0.60. Observou-se que participantes classificados
como respondentes à intervenção tiveram uma redução média de 5,1 pontos do PHQ-9 e 5,5 no GAD-7,
enquanto os não respondentes tiveram reduções médias de 2,4 e 1,8 respectivamente.

##### Limitações

A quantidade de dados faltantes era considerável e provavelmente não aleatória, o que limita
o desempenho de técnicas de imputação de dados. Os dados de testes usados na etapa final
foram coletados de uma população diferente da que gerou os dados de treinamento, podendo
ter prejudicado o desempenho preditivo dos modelos. O estudo não contou com uma base de comparação
realista (aqui autores sugerem comparar a precisão dos modelos com o julgamento de clínicos).


### A machine learning ensemble to predict treatment outcomes following an Internet intervention for depression

#### Autores

Rahel Pearson, Derek Pisner, Björn Meyer, Jason Shumake e Christopher G. Beevers.

#### Ano

2019.

#### Problema

Estudos apontam a eficácia de intervenções realizadas por Internet, mas poucos investigam a
resposta ao tratamento em nível individual.

#### Objetivo

Aplicar técnicas de *machine learning* para prever resultados de uma intervenção psicológica
voltada ao tratamento de depressão e realizada via Internet.

#### Metodologia

##### Participantes

Os dados foram coletados como parte do ensaio clínico que avaliava a eficácia do programa
Deprexis. Participaram do ensaior pessoas entre 18 e 55 anos que apresentassem sintomas moderados
ou mais graves de depressão (pontuação >= a 10 no instrumento QIDS).

##### Intervenção

O Deprexis é um tratamento para transtorno depressivo maior realizado via Internet e que
conta com um nível relativamente baixo de suporte de terapeutas. A intervenção consiste em
10 módulos de conteúdo cobrindo tópicos como ativação comportamental, reestruturação cognitva
exercícios de relaxamento, mindfulness e outros.

##### Desfechos observados

Foram observados os níveis de sintomas depressivos por meio dos instrumentos *Hamilton
Rating Scale for Depression* (HRSD), *Sheehan Disability Scale* (SDS) e a subescala
*Well-Being* do *Inventory of Depressive Symptoms* (IDAS Well-Being).

##### Plano de análise de dados

Os modelos de *machine learning* dos tipos *elastic net* e *random forest* foram treinados
utilizando dados clínicos e demográficos coletados antes da intervenção. A performance dos
modelos foi avaliada durante o treinamento usando a técnica de *nested cross-validation* ; o
método foi escolhido para evitar viéses otimistas observados em técnicas tradicionais de
*cross-validation* com amostras pequenas.

As previsões dos modelos foram então combinadas usando uma média aritmética simples, gerando
a previsão final do conjunto de modelos. O desempenho do conjunto de modelos foi comparado a
de um modelo de regressão linear treinado com o mesmo conjunto de dados (modelo de *benchmark*),
buscando observar as diferenças na variâncias explicadas pelas duas abordagens (o que os autores
chamam de 'ganho do modelo').

Os autores também avaliaram a importância de cada preditor inserido no modelo por meio de uma
ténica similar a SHAP, alterando o valor de uma variável por vez e observando as diferenças
produziadas no resultado.

Dados faltantes foram imputados usando a técnica de *miss forest*, que utilizada uma combinação
de regressões lineares e um algoritmo de *random forest* para gerar um valor artificial.

##### Resultados

O modelo de *benchmark* explicou 16,6% da variância observada nos resultados do HRSD; o conjunto
de modelos desenvolvidos explicou um adicional de 8%. Os preditores mais importantes foram: a
pontuação em escalas de depressão antes da intervenção, comorbidades, nível de funcionamento, nível
de engajamento com os módulos do Deprexis, credibilidade atribuída ao tratamento e disponibilidade
de terapeutas.

O conjunto de modelos também apresentou ganhos ao explicar a variância no nível de funcionamento e
no bem-estar dos participantes.

Ao analisar importância do uso de cada módulo do Deprexis, os autores observaram maior contribuição
dos módulos de relaxamento, aceitação, relacionamentos e reestruturação cognitiva.

##### Limitações

A amostra usada no estudo era pequena e relativamente homogênea, levando a um possível *overfitting*
do modelo aos dados. Sem acesso a dados de intervenções comparáveis, não é prever a respostas da
intervenção Deprexis em relação a uma alternativa.
