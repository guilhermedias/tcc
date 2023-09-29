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
Amanda C. Collins, George D. Price, Rosalind J. Woodworth e Nicholas C. Jacobson

#### Ano
2023

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
televisão e artigos da internet para participar de um estudo sobre felicidade.

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

