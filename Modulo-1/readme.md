# Analisando Dados do Tabnet
por Johnny Yamanaka

<br/>

## Introdução
O presente projeto é uma análise exploratório dos dados obtidos através do Tabnet - DATASUS, API com vários dados públicos do SUS.

## Objetivo
Diante da vastidão dos dados encontrados, foi delimitado que seriam analisado os seguintes dados, num período de 10 anos (2010-2020):
* Gastos do SUS;
* Óbitos;
* Taxa de mortalidade;
* Internações no SUS;
* Média de dias internados.

Os dados estão separados pelo estado onde foram computado essas informações. O primeiro desafio antes de realizar a análise propriamente dita, foi necessário realizar a limpeza e ajuste de alguns dados, etapas as quais foram documentadas no notebook desse projeto.

## Conclusões

Após a análise dos datasets, podemos chegar à algumas conclusões:
* A chegada da COVID19 foi um fator relevante para o aumento da taxa de mortalidade no SUS, especialmente nos estados da região Norte;
    * Na região sul os óbitos sobem no meio do ano (junho e julho) formando picos e regredindo após esse período. E após o início da pandemia esse a taxa de mortalidade salta para um novo patamar.
* Após o início da pandemia, a quantdidade de internações diminui drásticamente. Uma hipótese é que com as medidas restritivas que foram impostas em vários estados, a procura pelo médico ficou concentrado somente naqueles relacionados à COVID. Seria interessante ter a informação sobre a taxa de ocupação dos leitos para tentar validar essa hipótese. Outro ponto é acrescentar também a informação de 2021, para observar se a vacinação foi importante para diminuir esse dado;
* Observa-se que, nos estados onde o gasto aumenta os dias de internação tende a diminuir. Aqui precisamos fazer a ressalva de que esse gasto não é necessariamente investimento. Seria interessante procurar o valor do investimento para ver se essa tendência se mantém.
