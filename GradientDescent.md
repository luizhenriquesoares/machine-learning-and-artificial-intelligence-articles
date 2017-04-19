 ## Gradiente descendente e Cost Function 
 
 
  Quando falamos em modelos preditivos de machine learning, é comum associar a estatística e matemática e quão bem o modelo é preciso, em fazer previsões futuras sobre algo. 
Por trás de todo processo, os algoritmos de machine learning são instruções para equações matemática que descreve o relacionamento entre seus coeficientes. 
 
 
 O objetivo do algoritmo de ML é aprender um modelo que minimize os erros, A força motriz por trás do processo de otimização é a resposta para uma função interna, chamada de cost function. Também chamada  de função de perda (loss function)  
 
 
> A Cost function é uma função de avaliação, que mede quão bem seu modelo é preciso, a parti dos dados que você forneceu.  
 
 
Quando determinamos o nível de erro do algoritmo, comparando a previsão com seu valor real, que é dada pela MAE (Mean absolute Error), temos um valor, e quanto menor o valor como resultado desta função, corresponde  a uma melhor estimativa para os parâmetros desconhecidos x e y. 
 
 
Para minimizar a Cost Function, usamos um algoritmo de otimização com a descida do gradiente, que permite encontrar a melhor combinação de variáveis que minimiza a função de custo. 
 
 
 ## Gradiente descendente 
 
  ![Gradient descent](https://uploaddeimagens.com.br/images/000/894/803/full/grad.png?1492564492) 
  
Fazendo uma analogia, imagine uma pessoa em cima do topo de uma montanha, e para chegar ao destino, ela precisar descer, porém não sabe qual o melhor caminho, a medida que ela desce, para um lado ou outro, ela calcula qual a melhor descida, assim é como o grandient descent, funciona.  
 
 
Escolhendo aleatoriamente um novo ponto de partida, depois de ter encontrado um mínimo local, e repetir o processo iterativamente, mais cedo ou mais tarde, o mínimo global seja identificado 
 
## Implementação em python

> import random

> def random_w( p ):
    return np.array([np.random.normal() for j in range(p)])

> def hypothesis(X,w):
    return np.dot(X,w)

> def loss(X,w,y):
    return hypothesis(X,w) - y

> def squared_loss(X,w,y):
    return loss(X,w,y)**2

> def gradient(X,w,y):
    gradients = list()
    n = float(len( y ))
    for j in range(len(w)):
        gradients.append(np.sum(loss(X,w,y) * X[:,j]) / n)
    return gradients

> def update(X,w,y, alpha = 0.01):
    return [t - alpha*g for t, g in zip(w, gradient(X,w,y))]

> def optimize(X,y, alpha = 0.01, eta = 10**-12, iterations = 1000):
    w = random_w(X.shape[1])
    path = list()
    for k in range(iterations):
        SSL = np.sum(squared_loss(X,w,y))
        new_w = update(X,w,y, alpha = alpha)
        new_SSL = np.sum(squared_loss(X,new_w,y))
        w = new_w
        if k>=5 and (new_SSL - SSL <= eta and new_SSL - SSL >= -eta):
            path.append(new_SSL)
            return w, path
        if k % (iterations / 20) == 0:
            path.append(new_SSL)
    return w, path 
