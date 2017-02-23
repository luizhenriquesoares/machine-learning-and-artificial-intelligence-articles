
 
# Ferramentas - Machine Learning  
 
 
## PyStack 
* scikit-Learning  - http://scikit-learn.org/stable/ 
* pandas - http://pandas.pydata.org/ 
* numpy - http://www.numpy.org/ 
* matplotlib - http://matplotlib.org/ 
* scipy - https://www.scipy.org/ 
* seaborn - https://seaborn.pydata.org/ 
* statsModel - http://statsmodels.sourceforge.net/ 
* Dataset -> Estudos UCI Machine Learning  - http://archive.ics.uci.edu/ml/ 
 

# Tarefas de aprendizagem (Supervisionado) 
 
 ==============================================================================
 
## Regressão  
 
 
- Regressão Linear Simples e Múltipla 
- Decison Tree e suas variantes 
- Support Vector Machine - SVR  
- Ridge Regression 
- Lasso Regression 
- ElasticNet Regression 
- KNN 
 
 
# Métodos Ensamble Avançados 
 
 
- Gradient Boosting -> Também chamado de Stochastic Gradient Boosting, 
 
 
> Também chamado Stochastic Gradient Boosting, é um dos métodos Ensemble mais sofisticados. 
 
 
> Combinação de Boosting com Gradiente Descendente 
 
 
# XGBoost 
 
 
> O algoritmo XGBoost é uma extensão do GBM (Gradient Boosting Method) que permite trabalhar com multithreading em uma única máquina e processamento paralelo em um cluster de vários servidores. A principal vantagem do XGBoost sobre o GBM é sua capacidade de gerenciar dados esparsos. O XGBoost automaticamente aceita dados esparsos como input sem armazenar zeros na memória. 
 
 
## Avaliação do modelo de Regressão 
 
 
- SST, SSE, SSR, MSE, MSA, RMSE 
- Mean Absolute Error 
- Teste F de significância Global 
- Testes de significância Individuais 
- Coeficientes R2 e R2 Ajustado 
- Coeficientes de correlação  
- Confusion Matrix 
- Curva ROC 
- Resampling 
 
 
## Otimização 
 
 
- Gradiente Descendente -> Otimizar Cost Function. 
- Stocastic Grandiente Descendente 
- Cross validation -> Técnica de amostragem de dados.  
- Grid Search -> consiste em testar todas possibilidades de parâmetros de uma modelo (as vezes gera muito processamento) 
- Random Search -> alternativa para o Grid Search. 
- Cross Validation 
 
 
## K-fold com Cross Validation 
 
 
> Cross Validation é uma técnica que pode ser utilizada para avaliar a performance de um modelo com menos variância que a técnica de dividir os dados em treino/teste. Com esta técnica dividimos os dados em partes normalmente chamadas de k-folds (por exemplo k = 5, k = 10). Cada parte é chamada fold. O algoritmo é treinado em k-1 folds. Cada fold é usado no treinamento de forma repetida e um fold por vez. Após executar o processo em k-1 folds, podemos sumarizar a performance em cada fold usando a média e o desvio padrão Analytics). O resultado é normalmente mais confiável e oferece maior acurácia ao modelo. A chave deste processo está em definir o correto valor de k, de modo que o número de folds represente adequadamente o número de repetições necessárias. 
 
 
![Costfunction](https://uploaddeimagens.com.br/images/000/843/969/original/cross-validation.jpg?1487782505) 
 
 
# Pré-processamento 
 
 
Muitos algoritmos esperam receber os dados em um formato específico 
   Alguns algoritmos tem seu modelo de pré-processamento definido. 
 
 
> Pré-processamento é uma tarefa de preparo para otimizar seu modelo machine Learning 
 
 
Abaixo vamos listar algumas etapas das tarefas de pré-processamento: 
 
 
- Escala 
 
 
É umas das primeiras tarefas dentro do pré-processamento, é colocar seus dados na mesma escala, muitos do algoritmos vão se beneficiar com os resultados. 
 
 
> Esta etapa também é chamada de normalização, consiste em colocar os dados numa escala de 0 á 1. 
 
 
O scikit-Learning possui uma função para esta etapa chamada MinMaxScaler() 
 
 
# Padronização 
 
 
>Padronização é a técnica para transformar os atributos com distribuição Gaussiana (normal) e diferentes médias e desvios padrões em uma distribuição Gaussiana com a média igual a 0 e desvio padrão igual a 1 
 
 
scikit-Learning possui uma função para esta etapa, StandardScaler() 
 
 
 
 
# Normalização 
 
 
>No scikit-learn, normalização se refere a ajustar a escala de cada observação (linha) de modo que ela tenha comprimento igual a 1 (chamado vetor de comprimento 1 em álgebra linear). Este método de pré-processamento é útil quando temos datasets esparsos (com muitos zeros) e atributos com escala  
muito variada. Útil quando usamos algoritmos de redes neurais ou que usam medida de distância, como KNN. O scikit-learn possui uma função para esta etapa, chamada Normalizer(). 
 
 
# Feature Selection 
 
 
>A etapa de Feature Selection é onde selecionamos os atributos (variáveis) que serão melhores candidatas a variáveis preditoras. O Feature Selection nos ajuda a reduzir o overfitting (quando o algoritmo aprende demais), aumenta a acurácia do modelo e reduz o tempo de treinamento. 
- SelectKBest  
 
 
## Eliminação Recursiva de Atributos 
 
 
> Esta é outra técnica para seleção de atributos, que recursivamente remove os atributos e constrói o modelo com os atributos remanescentes. Esta técnica utiliza a acurácia do modelo para identificar os atributos que mais contribuem para prever a variável alvo. Em inglês esta técnia é chamada Recursive Feature Elimination (RFE). 
 
 
 
 
## Método Ensemble para Seleção de Variáveis 
 
 
- Bagged Decision Tree  
 
 
## Feature Extraction 
 
 
- Principal Component Analysis (PCA) (Redução de Dimensionalidade) 
 
 
# Classificação 
 
 
- Nearest Neighbours (KNN) 
- Decision Tree 
- Random Forest 
- Métodos Esemble (Bagging, Extra Tree, AdaBoost) 
- Naive Bayes 
- Support Vector machine (Função Kernel Trick para dados não linear ou linear) 
 
 
## Métricas para Algoritmos de Classificação 
 
 
- Acurácia 
- Curva ROC 
- Confusion Matrix 
- Logarithmic Loss 
 
 
# Não - Supervisionado 
 
 
## Clustering 
 
 
- K-Mean 
- Mean Shift 
- Affinity Propagation 
- K-Mean++ 
- DBSCAN 
 
 
# Redes Neurais 
 
 
* Peceptron com multicamadas - Backpropagation 
* Redes feedforward 
* Redes CNN (Covolucionárias) - Reconhecimento de imagem 
* Redes RNN (Redes Neurais Recorrentes) - Processamento de Voz... Linguagem Natural 
* LSTM - Long Short-Term Memory 
 
 
# Função Ativação 
 
* sigmoid  
* softMax  

## Deep Learning 
 
* TensorFlow - No Backend 
* Keras - No Front-end 
* Theano 

# Referências

* https://github.com/luizhenriquesoares/data-science-ipython-notebooks
* https://pt.coursera.org/learn/machine-learning
* http://www.datascienceacademy.com.br/
* https://www.kaggle.com/
* http://libgen.io/ -> baixar livros

# Github

* https://github.com/rasbt
* https://github.com/hmason
* https://github.com/amueller
* https://github.com/rdpeng
* https://github.com/jakevdp


# Books

* https://github.com/rasbt/python-machine-learning-book
* https://github.com/rasbt/deep-learning-book 
* Python Machine Learning - Sebastian Raschka
* Andreas C. Müller, Sarah Guido-Introduction to Machine Learning with Python_ A Guide for Data Scientists-O’Reilly Media (2016)

# Video

* Deep Learning

> Deep Learning in Practice: Speech Recognition and Beyond

 http://events.technologyreview.com/video/watch/andrew-ng-deep-learning/?utm_medium=native_social&utm_source=facebook&utm_campaign=emtech_digital_reg&utm_term=artificial_intelligence&utm_content=ng_video
