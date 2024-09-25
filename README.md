# Análise sobre o **IDHM** as cidades brasileiras

A ideia desse pequeno projeto da disciplina de *Machine Learning* é fazer uma análise usando de diversos modelos de regressão sobre o dataset *Brazilian Cities*, verificando o IDHM de cada cidade e indicando o modelo de regressão que melhor se adequa.

## Metodologia

Analisando o *dataset*, chegou-se a conclusão que se tratava de um modelo de regressão, já que nosso objetivo é uma predição numérica com base em dados já rotulados.

Para isso, resolveu-se analisar cinco modelos de regressão que vimos ao longo da disciplina de *machine learning*:

- Regressão Linear
- *K-Nearest Neighbors*
- Árvore de Decisão
- *Random Forest*
- *Extremely Randomized Trees*

E, para fins científicos, analisar os resultados dos modelos treinados em cinco etapas, rotuladas da seguinte forma:

- **Etapa 1**: dados faltantes foram preenchidos, dados categóricos foram transformados em numéricos e removeu-se colunas de alta correlação com o atributo alvo - como outros tipos de IDHM.
- **Etapa 2**: tudo que foi aplicado na etapa 1 e a remoção de *outliers*
- **Etapa 3**: tudo que foi aplicado na etapa 2 e a normalização dos dados
- **Etapa 4**: tudo que foi aplicado nas etapas anteriores
- **Etapa 5**: tudo que foi aplicado nas etapas anteriores e a remoção de colunas com baixa correlação com o atributo alvo, que árbitrariamente foi definido como valores abaixo de 0.1

## Resultados obtidos (score)

| Modelo | Etapa 1 | Etapa 2 | Etapa 3 | Etapa 4 | Etapa 5 |
|--------|---------|---------|---------|---------|---------|
| *Linear Regression* | 0.8289 | 0.8155 | 0.8215 | 0.8222 | 0.8155 |
| *K-Nearest Neighbors* | 0.4593 | 0.4616 | 0.8119 | 0.8194 | 0.8280 |
| Árvore de Decisão | 0.8051 | 0.8004 | 0.8071 | 0.8010 | 0.8002|
| *Random Forest* | 0.8635 | 0.8591 | 0.8690 | 0.8706 | 0.8677 |
| *Extra Trees* | 0.8253 | 0.8216 | 0.8309 | 0.8378 | 0.8364 |

## Links úteis

- [Dataset Brazilian Cities](https://www.kaggle.com/datasets/crisparada/brazilian-cities), disponível no Kaggle
