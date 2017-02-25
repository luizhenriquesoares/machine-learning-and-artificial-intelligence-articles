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

### Reduzir os valores dos coeficientes:

> Nesse caso, ajustamos o modelo com todas as variáveis, porém os coeficientes passam a receber pesos reduzindo assim variância dos dados.

Esse Método é conhecido como <b>Regularização</b>, dependendo do tipo de Regularização, os coeficientes podem chegar a 0.

> A Regularização é um método que colocamos pesos sobre determinados coeficientes, conseguindo minimiza-los para encontrar um modelo adequado.

Os dois grupos principais da Regularização é <b><i>Rigde</i></b> e <i><b>LASSO</i></b>:

# Rigde