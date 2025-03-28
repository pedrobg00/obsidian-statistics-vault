Seja $X$ uma variável aleatória discreta com função de probabilidade $P_X(x)$, a esperança (ou média, ou valor esperado) de $X$ é definida como

$$


E(X) = \sum_{x \in \mathrm{Im}(X)} x.P(X=x)


$$

onde $\mathrm{Im}(X)$ representa o conjunto de todos os valores possíveis que a variável aleatória $X$ pode assumir. Esta fórmula calcula a soma ponderada dos valores possíveis de $X$, onde cada valor é multiplicado pela sua respectiva probabilidade.

Por exemplo, considere uma v.a. discreta $X$ que representa o número de caras ao lançar duas moedas justas. As possíveis saídas são: 0 caras (ambas coroas), 1 cara (uma cara e outra coroa), ou 2 caras (ambas caras). A função de probabilidade para cada resultado é:

$$


P(X=0) = \frac{1}{4}, \quad P(X=1) = \frac{1}{2}, \quad P(X=2) = \frac{1}{4}


$$

A esperança $E(X)$ pode ser calculada como:

$$


E(X) = 0 \cdot P(X=0) + 1 \cdot P(X=1) + 2 \cdot P(X=2)


$$

$$


E(X) = 0 \cdot \frac{1}{4} + 1 \cdot \frac{1}{2} + 2 \cdot \frac{1}{4}


$$

$$


E(X) = 0 + \frac{1}{2} + \frac{1}{2} = 1


$$

Portanto, a esperança da v.a. $X$ neste exemplo é 1.

## Esperança De Funções De Variáveis Aleatórias Discretas

Agora que entendemos como calcular a esperança de uma variável aleatória discreta, vamos explorar como calcular a esperança de uma função dessa variável. Seja $g(X)$ uma função qualquer definida em $\mathrm{Im}(X)$. A esperança da função $g(X)$ é dada por:

$$
E(g(X)) = \sum_{x \in \mathrm{Im}(X)} g(x).P_X(x)
$$

Esta fórmula indica que a esperança de uma função de variável aleatória é a soma ponderada dos valores da função $g$ em cada possível valor de $X$, onde os pesos são as respectivas probabilidades.

### Exemplo: Função Quadrática

Considere o mesmo exemplo anterior, onde $X$ representa o número de caras ao lançar duas moedas justas. Agora, vamos calcular a esperança da função quadrática $g(X) = X^2$. As possíveis saídas e suas probabilidades são:

$$
P(X=0) = \frac{1}{4}, \quad P(X=1) = \frac{1}{2}, \quad P(X=2) = \frac{1}{4}
$$

A esperança de $g(X)$ pode ser calculada como:

$$
E(g(X)) = E(X^2) = 0^2 \cdot P(X=0) + 1^2 \cdot P(X=1) + 2^2 \cdot P(X=2)
$$

Substituindo os valores, temos:

$$
E(X^2) = 0^2 \cdot \frac{1}{4} + 1^2 \cdot \frac{1}{2} + 2^2 \cdot \frac{1}{4}
$$

$$
E(X^2) = 0 + \frac{1}{2} + \frac{4}{4} = \frac{1}{2} + 1 = \frac{3}{2}
$$

Portanto, a esperança da função quadrática $g(X) = X^2$ neste exemplo é $\frac{3}{2}$.

### Propriedades Importantes

1. **Linearidade**: A esperança é uma operação linear, ou seja,

   $$
   E(aX + b) = aE(X) + b \quad \text{para constantes } a \text{ e } b.
   $$

2. **Esperança de Função Constante**: Se $g(X) = c$ (uma constante), então

   $$
   E(g(X)) = E(c) = c.
   $$

3. **Esperança da Variável Aleatória Elevada ao Quadrado**:

   $$
   \mathrm{Var}(X) = E(X^2) - [E(X)]^2,
   $$

   onde $\mathrm{Var}(X)$ é a variância de $X$.

Estas propriedades são úteis para simplificar cálculos e entender melhor as relações entre diferentes funções de variáveis aleatórias.

