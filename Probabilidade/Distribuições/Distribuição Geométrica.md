Considere que vamos realizar ensaios independentes de Bernoulli até a ocorrência do primeiro sucesso. Cada ensaio é um experimento binomial, onde há apenas dois possíveis resultados: sucesso ou fracasso. A probabilidade de sucesso em cada ensaio é denotada por $p$, e consequentemente, a probabilidade de fracasso é $1 - p = q$.

## Distribuição Geométrica

A distribuição geométrica descreve o número de ensaios necessários para obter o primeiro sucesso. Seja $X$ a variável aleatória que representa o número de ensaios até o primeiro sucesso. A função de probabilidade da distribuição geométrica é dada por:

$$
P(X = k) = (1 - p)^{k-1}p, \quad k = 1, 2, 3, \ldots
$$

Onde:

- $k$ é o número de ensaios até o primeiro sucesso.
- $p$ é a probabilidade de sucesso em cada ensaio.

## Exemplo

Suponha que uma moeda justa seja lançada repetidamente até obter a primeira cabeça (sucesso). A probabilidade de obter uma cabeça ($p = 0.5$) e a probabilidade de obter uma coroa ($q = 0.5$) são iguais.

- A probabilidade de obter o primeiro sucesso no primeiro lançamento é:

  $$
  P(X = 1) = (1 - 0.5)^{1-1} \cdot 0.5 = 0.5
  $$

- A probabilidade de obter o primeiro sucesso no segundo lançamento é:

  $$
  P(X = 2) = (1 - 0.5)^{2-1} \cdot 0.5 = 0.5^2 \cdot 0.5 = 0.25
  $$

## Parâmetros E Propriedades

A distribuição geométrica é completamente determinada pelo único parâmetro $p$, que representa a probabilidade de sucesso em cada ensaio.

- **Esperança (Média):** A esperança da variável aleatória $X$ é:

  $$
  E(X) = \frac{1}{p}
  $$

- **Variação:** A variância da variável aleatória $X$ é:

  $$
  Var(X) = \frac{q}{p^2} = \frac{1 - p}{p^2}
  $$

## Aplicações Práticas

A distribuição geométrica tem diversas aplicações em problemas reais, como:

- **Probabilidade de obter o primeiro sucesso em experimentos repetidos:** Por exemplo, a probabilidade de um jogador de basquete marcar seu primeiro arremesso no jogo.
- **Tempo até a ocorrência do primeiro evento específico:** Como o tempo até que um cliente entre em uma loja após o início da operação.
