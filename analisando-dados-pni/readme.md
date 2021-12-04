# Analisando Dados do PNI  
por Johnny Yamanaka

<br/>

## Introdução  
Neste projeto analisaremos dessa vez a base de dados do [PNI](http://tabnet.datasus.gov.br/cgi/tabcgi.exe?pni/cnv/cpniuf.def) (Programa Nacional de Imunização) fornecida pelo DATASUS. Esse dataset traz a cobertura vacinal por estado e separado por ano. A covertura de vacinação, segundo o [Centro de Liderança Pública - CLP](https://www.clp.org.br/cobertura-vacinal-o-que-e-como-esta-e-por-que-e-tao-importante/) é a porcentagem de pessoas completamente vacinadas dentro do total de pessoas que precisam ser vacinadas. Esse dado é muito importante porque, com a imunização pode-se prevenir ou até erradicar doenças, como é o caso da [Varíola, Poliomielite](https://vacinas.com.br/blog/doencas-erradicadas-com-a-vacinacao/).  

## Os Dados
Além dos dados do PNI, esse projeto traz também os dados como taxa de óbito e gastos do SUS, todas anualizadas, compreendo o período de 2018 a 2018. Não foi possível trazer dados mais atuais pois o DATASUS só disponibiliza até o momento da execução desse projeto dados até set/19.

## Objetivo  
Com os dados à disposição, foi levantado quatro hipóteses para explorarmos:

* H1: Cobertura vacinal maior está relacionado à taxa de mortalidade menor.
* H2: Cobertura vacinal maior está relacionado à gastos menor do sus.
* H3: Ao longo dos ultimos anos, a cobertura vacinal diminuiu em todo território nacional.
* H4: A região sudeste possui a maior cobertura vacinal que as outras regiões.

## Conclusão  

Das 4 hipóteses levantadas inicalmente, 3 delas se mostraram inconclusivas para os dados que temos. Isso porque, no dataset com as despesas do sus não há discriminação do destino dos gastos, bem como no dataset de taxa de óbito não é somente para as doenças que podem ser evitadas pela vacina. Dentro do próprio DATASUS é possível realizar alguns filtros, no futuro pode ser interessante refazer as análises com dados mais delimitados. Seria bom também ter os dados da cobertura vacinal atualizada, pelo menos até 2020 para podermos ver o efeito da pandemia dos dados.
