# Viés e Variância (bias and variance)

 - Quando construimos um modelo que generaliza incorretamente particularidades dos dados, temos um problema conhecido como overfitting

    Uma forma ilustrativa de compreender tal fenômeno, é separar o erro de generalização em viés (bias) e variâcia (variance).

     ## Viés
    

    > Viés é a tendência do modelo aprender consistentemente uma generalização incorreta.

    ## Variância

    > Variância é a tendência de se aprender fatos aleatórios independentemente do sinal real.



    Um modelo muito complexo tem alta variância, por ser capaz de aprender padrões que não possam ser reais. Isso faz com que os modelos mais complexos sejam a única alternativa
    
     ## Formula Cost function
     ![vies](https://uploaddeimagens.com.br/images/000/837/287/original/bies.png)
 

    Ao fazer previsões devemos separar nossa amostra em dados de treino e a outra parte que vamos avaliar a qualidade da previsão, que são os dados de teste.
