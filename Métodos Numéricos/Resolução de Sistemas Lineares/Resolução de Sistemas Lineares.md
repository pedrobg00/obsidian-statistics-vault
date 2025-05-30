---
dg-publish: true
dg-show-local-graph: true
---

%% Begin Waypoint %%

- [[Resolução de Sistemas Lineares]]
	- [[Fatoração LU]]
	- [[Método de Eliminação de Gauss]]
	- [[Método de Gauss-Jacobi]]
	- [[Método de Gauss-Seidel]]
	- [[Métodos Diretos - Sistema Triangular]]
	- [[Métodos Iterativos]]
	- [[Teorema Condição Suficiente de Converência do Método de Gauss-Jacobi]]

%% End Waypoint %%

## Linearidade de Funções

Uma função $f$ é dita linear se satisfaz as seguintes propriedades:

1. **Aditividade**: Para quaisquer valores $x$ e $y$, temos que
$$
f(x + y) = f(x) + f(y).
$$
2. **Homogeneidade de grau 1**: Para qualquer escalar $c$ e valor $x$, temos que
$$
f(cx) = cf(x).
$$

A combinação dessas duas propriedades resulta na forma geral de uma função linear, que pode ser expressa como:

$$
f(x) = ax + b,
$$

onde $a$ e $b$ são constantes. Aqui, $b$ é o intercepto y (o valor da função quando $x=0$), enquanto $a$ é a inclinação da reta.

### Exemplos de Funções Lineares

1. **Função Constante**: A função $f(x) = 5$ é linear com $a = 0$ e $b = 5$. Embora seja uma função linear, ela não satisfaz a propriedade de inclinação (aditividade).
2. **Função de Retas**: A função $g(x) = 3x - 4$ é um exemplo clássico de uma função linear com $a = 3$ e $b = -4$. Ela representa uma reta com inclinação positiva.
