# Projeto de Otimização de ARPU com LGBM Regressor

## Descrição

Este projeto tem como objetivo otimizar o **ARPU (Average Revenue Per User)** utilizando um modelo de **LGBM Regressor**. A otimização é feita com base em diferentes combinações de canais de marketing e tipos de ofertas, com o intuito de maximizar o ARPU.

A abordagem envolve o uso de um modelo preditivo treinado para identificar quais combinações de variáveis (canais e ofertas) resultam no maior valor de "amount". Este processo é feito em um conjunto de validação, onde testamos todas as combinações possíveis e escolhemos a mais vantajosa.

## Estrutura do Projeto

- **`modelo01.ipynb`**: Contém o código principal para treinar e testar o modelo LGBM Regressor.
- **`database_treat.ipynb`**: Contém o código de tratamento da base inicial por meio de PySpark.
- **`requirements.txt`**: Lista as dependências do projeto.


## Observações

O modelo apresenta um possível overfitting. Para minimizá-lo poderíamos ter feito uma feature engineering mais robusta, como por exemplo ter criado cluster com KMeans antes de rodar o LGBM Regressor, assim como testar com mais dados. Além disso uma otimização de hiperparâmetro docando na redução de overfitting também seria válida. Com mais dados e mais possibilidades de feature engineering também seria possível a utilização de um modelo em rede neural com maior flexibilidade para evitar o overfitting. 
