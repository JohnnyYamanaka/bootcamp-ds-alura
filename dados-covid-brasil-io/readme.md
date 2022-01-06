# Dados do Covid - Brasil.IO
# Predição de Casos em São José dos Campos (SP)
por [Johnny Yamanaka](https://www.linkedin.com/in/johnny-yamanaka/)

## Introdução
Não é segredo para ninguém que com a pandemia do novo corona vírus tivemos vários desafios, e uma delas foi o acompanhamento da evolução dessa doença na nossa sociedade. Seja por causa da falta de organização, estruturas precárias para testagem e rastreio de contágio, pode-se dizer que o Brasil enfrentou inicialmente a pandemia de forma inadequada. Os dados são geradas de forma independente pelas secretarias ou ministérios de saúde dos três níveis do executivo, o que dificulta a tabulação dos dados. Nesse contexto, o [Brasil.IO](https://brasil.io/dataset/covid19/caso_full/) vai atrás, consolida e disponibiliza esses dados públicos a quem interessar.

## Objetivo
O presente projeto tem como objetivo desenvolver um modelo para prever a quantidade de novos casos de covid na cidade de de São José dos Campos, localizado na região do vale do paraíba, à 90km da capital paulista. A escolha dessa cidade se deve pelo tamanho da sua população ser a maior da região (730 mil) e concentrar uma porção relevantes dos casos.

## Resultado
Durante o processo de desenvolvimento foram criadas vários modelos, e a performance foi melhorando na medida em que os parâmetros eram ajustados.

| model        | mae    | rmse   | r2   |
|--------------|--------|--------|------|
| modelo_base  | 111.59 | 157.40 | 0.21 |
| modelo2      | 106.56 | 156.00 | 0.22 |
| modelo3      | 105.34 | 154.30 | 0.24 |
| modelo4      | 105.27 | 154.22 | 0.24 |
| modelo5      | 105.68 | 154.77 | 0.23 |
| modelo_final | 74.09  | 119.65 | 0.54 |

Esses resultados ainda podem ser melhorados com aplicação de mais técnicas, como analisar e tratar os outliers, normalizar os dados e realizar mais ajustes nos parâmetros do modelo.

## Conclusão
O modelo final erra em média (MAE) 74 casos, para mais ou menos, o que representa ~0,1% da população da cidade, mas esse desempenho ainda pode ser melhorado sem atingir o sobreajuste (overfitting). Outro ponto que precisamos destacar é que, assim como em todo Brasil os casos podem estar subnotificados, além da falta de regularidade na emissão dos boletins de casos por parte da secretaria municipal. Vemos isso porque quando observamos o dataset, vemos que temos dados consistentes somente até outubro/21. Para que possamos modelar melhor o problema e controlar essa doença, é necessário que tenhamos dados mais consistentes e atualizados.
