# Análise sobre o **IDHM** as cidades brasileiras

A ideia desse pequeno projeto da disciplina de *Machine Learning* é fazer uma análise usando de diversos modelos de regressão sobre o dataset *Brazilian Cities*, verificando o IDHM de cada cidade e indicando o modelo de regressão que melhor se adequa.

## Resultados obtidos (score)

| Modelo | Sem pré-processamento | Sem outliers | Normalizado | Pré-processamento completo | Tudo que tem direito |
|--------|--------------------|----------|----------|------------|--|
| *Linear Regression* | 0.8289 | 0.8152 | 0.8215 | 0.8222 | 0.8155 |
| *K-Nearest Neighbors* | 0.4593 | 0.8485 | 0.8119 | 0.8194 | 0.8280 |
| Árvore de Decisão | 0.8051 | 0.8406 | 0.8071 | 0.8010 | 0.8002|
| *Random Forest* | 0.8635 | **0.9018** | 0.8690 | 0.8706 | 0.8677 |
| *Extra Trees* | 0.8253 | 0.8466 | 0.8309 | 0.8378 | 0.8364 |




## Links úteis

- [Dataset Brazilian Cities](https://www.kaggle.com/datasets/crisparada/brazilian-cities), disponível no Kaggle