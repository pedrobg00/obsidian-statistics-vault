## Introdução Às Variáveis Aleatórias

As variáveis aleatórias são fundamentais na teoria da probabilidade e estatística, servindo como a ponte entre o mundo dos números determinísticos e o dos eventos incertos. Elas permitem modelar situações onde os resultados não são conhecidos com certeza antes de ocorrerem.

### Definição

Uma variável aleatória é uma função que associa um valor numérico a cada resultado possível em um espaço amostral $\Omega$. Em notação matemática, se $X$ for uma variável aleatória e $\omega \in \Omega$, então $X(\omega)$ representa o valor numérico associado ao resultado $\omega$.

### Exemplos

1. **Tirar um Dado**: Considere o espaço amostral $\Omega = \{1, 2, 3, 4, 5, 6\}$, onde cada número representa a face de um dado que pode aparecer ao lançá-lo. Se $X$ for a variável aleatória que representa o valor do resultado, então $X(\omega) = \omega$, para $\omega \in \Omega$. Por exemplo, se $\omega = 3$, então $X(3) = 3$.

2. **Tempo de Chegada**: Considere um sistema onde os clientes chegam a uma loja com tempos variáveis. Se $T$ for a variável aleatória que representa o tempo de chegada do próximo cliente, então $T(\omega)$ pode assumir qualquer valor numérico positivo dependendo da situação.

3. **Temperatura**: Suponha que estamos interessados na temperatura diária em um determinado local. Se $Y$ for a variável aleatória que representa a temperatura no dia $\omega$, então $Y(\omega)$ pode assumir qualquer valor numérico dentro de uma faixa específica, dependendo das condições climáticas.

### Tipos De Variáveis Aleatórias

- **Discretas**: Têm um número contável de valores possíveis. Por exemplo, o número de carros vendidos em um dia.

  $$

X(\omega) = \begin{cases}

  0 & \text{se não vendeu nenhum carro} \\

  1 & \text{se vendeu um carro} \\

  2 & \text{se vendeu dois carros} \\

  \vdots

  \end{cases}

$$
- **Contínuas**: Podem assumir qualquer valor numérico dentro de um intervalo. Por exemplo, a altura de uma pessoa.

  
$$

Y(\omega) = \text{altura da pessoa em metros}

$$
### Função De Distribuição Acumulada (FDA)

A função de distribuição acumulada $F_X(x)$ de uma variável aleatória discreta $X$ é definida como:
$$

F_X(x) = P(X \leq x)

$$
Para a variável aleatória contínua $Y$, a FDA é dada por:
$$

F_Y(y) = P(Y \leq y)

$$
Essa função descreve a probabilidade de que o valor da variável aleatória seja menor ou igual a um certo ponto.

### Esperança E Variância

- **Esperança**: É a média esperada dos valores que uma variável aleatória pode assumir. Para uma variável discreta $X$, é dada por:
$$

E[X] = \sum_{x} x \cdot P(X = x)

$$
  Para uma variável contínua $Y$, é dada por:

  
$$

E[Y] = \int_{-\infty}^{\infty} y \cdot f_Y(y) \, dy

$$
- **Variância**: Mede a dispersão dos valores em torno da média. É definida como o quadrado da desvio padrão e para uma variável discreta $X$ é:

  
$$

\text{Var}(X) = E[(X - E[X])^2] = \sum_{x} (x - E[X])^2 \cdot P(X = x)

$$
  Para uma variável contínua $Y$, a variância é:

  
$$

\text{Var}(Y) = E[(Y - E[Y])^2] = \int_{-\infty}^{\infty} (y - E[Y])^2 \cdot f_Y(y) \, dy

$$
Essas medidas são essenciais para entender e quantificar a tendência central e a dispersão dos dados associados às variáveis aleatórias.

## Espaço De Probabilidade Produzido Por Variável Aleatória

[[Espaço De Probabilidade Produzido Por Variável Aleatória]]

## Tipos De Variáveis Aleatórias
### Variável Aleatória Discreta

Seja $X: \Omega \to \mathbb{R}$ uma variável aleatória definida em um espaço amostral $\Omega$ equipado com uma probabilidade $P$. A medida induzida por $X$ é denotada por $P_X$, e a função de distribuição acumulada (FDA) associada a $X$ é dada por $F_X(x)$.

Dizemos que $X$ é uma variável aleatória discreta se sua função de distribuição acumulada $F_X(x)$ satisfaz as seguintes propriedades:

#### 1. Definição Da FDA Para VA Discreta
$$

F_X(x) = P(X \leq x)

$$
Esta expressão representa a probabilidade de que o valor da variável aleatória $X$ seja menor ou igual a um determinado ponto $x$.

#### 2. Característica Principal De VA Discretas

A FDA de uma variável aleatória discreta é uma função constante por partes, o que significa que ela salta em certos pontos específicos correspondentes aos valores possíveis da variável aleatória.

#### 3. Exemplo

Considere $X$ como a variável aleatória que representa o número de caras ao lançar duas moedas justas. Os valores possíveis de $X$ são 0, 1 e 2.  

- Para $x < 0$, $F_X(x) = 0$.  

- Para $0 \leq x < 1$, $F_X(x) = P(X = 0) = \frac{1}{4}$.  

- Para $1 \leq x < 2$, $F_X(x) = P(X = 0) + P(X = 1) = \frac{1}{4} + \frac{1}{2} = \frac{3}{4}$.  

- Para $x \geq 2$, $F_X(x) = 1$.  

Portanto, a FDA de $X$ é:  
  
$$

F_X(x) =

\begin{cases}

0 & \text{se } x < 0 \\

\frac{1}{4} & \text{se } 0 \leq x < 1 \\

\frac{3}{4} & \text{se } 1 \leq x < 2 \\

1 & \text{se } x \geq 2

\end{cases}

$$
  
#### 4. Interpretação

A função constante por partes da FDA reflete a natureza discreta dos valores que $X$ pode assumir, com saltos significativos em cada valor possível de $X$.

#### 5. Consequências Práticas

- A probabilidade de $X$ assumir um valor específico é dada pelo salto na FDA.  
- Por exemplo, a probabilidade de $X = 1$ é:  
$$

P(X = 1) = F_X(1^+) - F_X(1^-) = \frac{3}{4} - \frac{1}{4} = \frac{1}{2}

$$
- Onde $F_X(1^+)$ e $F_X(1^-)$ representam os valores da FDA à direita e à esquerda de 1, respectivamente.
