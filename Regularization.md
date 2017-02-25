# Regularização

Regularização é um tema avançado em <i>machine learning</i>, e muito usado por quem já domina regressão linear.

Regularização é usado quando temos um dataset com uma grande quantidade de atributos, isso significa que muitas
variáveis seriam ajustas e o modelo ficaria super estimado com uma variância infinita, sendo inviável o método
dos mínimos quadrados.

## Métodos de redução de variáveis

Temos basicamento 3 métodos para redução da variância quando o número de variáveis é maior que o número de observações:

* Seleção de um subconjunto de coeficientes.
* Reduzir a dimensão 
* Reduzir o valor dos coeficientes (Regularização)