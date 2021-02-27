# Machine Learning Previsão Demanda

Modelo de Machine Learning para previsão de demanda de item da loja.

São dados 5 anos de dados de vendas de itens da loja com 50 itens diferentes em 10 lojas diferentes.

O objetivo é prever 3 meses a nível de item vendido com dados de diferente loja.

### Descrição do arquivo:

- train.csv - Dados de Treino; 
- test.csv - Dados de Teste; 
- sample_submission.csv - Arquivo no formato correto para o envio;

### Campos do arquivo:

- date - Data da venda - Esses dados não tem informação de feriado ou de dia que a loja ficou fechada; 
- store - Identificação da Loja; 
- item - Identificação do item; 
- sales - Número de itens vendidos de uma determinada loja e em uma determinada data;



Nesse projeto foi usado três modelos: XGBoostRegressor, LGBMRegressor e CatBoostRegressor onde o modelo da CatBoost se saiu melhor que os outros.

A métrica de avaliação usada nesse projeto foi a MAPE (Erro Absoluto Médio Percentual) que mede a média do erro percentual em relação ao valor real com o valor previsto.

  

Para melhorar os resultados poderia testar:

- Usar outros algoritmos como ARIMA, Prophet do Facebook ou Rede Neural LSTM (Long Short Term Memory);

- Efetuar normalização dos dados;

- Combinação de modelos;


Link Dataset Kaggle: https://www.kaggle.com/c/demand-forecasting-kernels-only/data
