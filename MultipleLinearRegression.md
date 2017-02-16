# Regressão Linear Multipla 

- Na Regressão Linear Multipla, temos um problema que é a alta colinearidade, que é a alta taxa de correlação com as variávies preditoras.
 
    > Quanto maior a colinearidade maior a variância, formando o modelo com overfitting.

## Como avaliar ou interpretar um modelo de regressão?

* Teste F de significância Global
* Testes de significância Individuais
* Coeficientes R2 e R2 Ajustado
* Coeficientes

 Teste F de significância Global, permite interpretar o modelo de regressão linear com o teste do valor-p 
 
 >o modelo é útil ?

 O teste do valor-p ajuda a interpretar se há evidência estátisticas. Se o valor-p do teste F, for menor que (F < 0,05), há evidências estátisticas, que pelo menos
uma variável do modelo tem relação com a variável target.

Caso o valor maior (F > 0,05), seu modelo não tem dados suficiente ou seus dados estão incorretos, para prever o a saída do do seu modelo.

## Em Regras Gerais:

> O modelo é útil para prever se o valor-p do teste F é menor que 0,05

## Objetivo

> O objetivo da regressão é encontrar os coeficientes que permitem construir a equação de regressão e fazer as previsões