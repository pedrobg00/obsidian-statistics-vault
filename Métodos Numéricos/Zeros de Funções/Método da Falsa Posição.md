O método da falsa posição, também conhecido como método dos segmentos ou método das retas secantes, é um algoritmo numérico utilizado para encontrar raízes aproximadas de uma função contínua. Este método combina a simplicidade do método das retas secantes com a eficiência do método da bisseção.

## Aplicação E Contexto

Este método é especialmente útil quando se tem duas aproximações iniciais $a$ e $b$ tais que $f(a)$ e $f(b)$ têm sinais opostos, garantindo assim a existência de pelo menos uma raiz no intervalo $[a, b]$. A função $f(x)$ deve ser contínua em todo o intervalo considerado.

## Formulação Do Método

O método da falsa posição envolve iterativamente reduzir o tamanho do intervalo onde a raiz está localizada. Na cada iteração, uma nova aproximação para a raiz é calculada usando a fórmula:

$$
x_n = \frac{a_{n-1}f(b_{n-1}) - b_{n-1}f(a_{n-1})}{f(b_{n-1}) - f(a_{n-1})}
$$

onde $a_{n-1}$ e $b_{n-1}$ são os valores dos extremos do intervalo atual, e $x_n$ é a nova aproximação.

## Exemplo De Aplicação

Considere a função $f(x) = x^3 - 2x - 5$. Sejam as aproximações iniciais $a_0 = 1$ e $b_0 = 2$, pois $f(1) < 0$ e $f(2) > 0$.

- **Iteração 1:**

  $$

  x_1 = \frac{1 \cdot f(2) - 2 \cdot f(1)}{f(2) - f(1)} = \frac{1 \cdot (8 - 3) - 2 \cdot (-2 - 5)}{(8 - 3) - (-2 - 5)} = \frac{5 + 14}{11 + 7} = \frac{19}{18} \approx 1.056


$$

- **Iteração 2:**

  $$

  x_2 = \frac{1 \cdot f(1.056) - 1.056 \cdot f(1)}{f(1.056) - f(1)}

$$
  Calculando $f(1.056)$:
  $$

  f(1.056) = (1.056)^3 - 2(1.056) - 5 \approx -4.87

$$
  Então:

$$

  x_2 = \frac{1 \cdot (-4.87) - 1.056 \cdot (-2)}{-4.87 - (-2)} = \frac{-4.87 + 2.112}{-4.87 + 2} = \frac{-2.758}{-2.87} \approx 0.963

$$
