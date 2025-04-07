## Definição

Uma série de Taylor de uma função $f(x)$ em torno de um ponto $x = a$ é dada por:

$$
f(x) \approx f(a) + \frac{f'(a)}{1!}(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \cdots + \frac{f^{(n)}(a)}{n!}(x-a)^n
$$

Aqui, $f^{(n)}(a)$ representa a $n$-ésima derivada de $f(x)$ avaliada em $x = a$. A série completa é:

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!}(x-a)^n
$$

## Exemplos

1. **Exponencial:**
   A função exponencial $e^x$ tem uma série de Taylor em torno do ponto $x = 0$ (também conhecida como série de Maclaurin):

   $$
   e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!}
   $$

2. **Cosseno:**
   A função cosseno $\cos(x)$ tem a seguinte série de Taylor em torno do ponto $x = 0$:

   $$
   \cos(x) = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n}}{(2n)!}
   $$

3. **Seno:**
   A função seno $\sin(x)$ tem a seguinte série de Taylor em torno do ponto $x = 0$:

   $$
   \sin(x) = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n+1}}{(2n+1)!}
   $$

## Aplicações

As séries de Taylor são amplamente utilizadas em cálculos numéricos, onde elas permitem aproximar funções complexas por polinômios mais simples. Além disso, essas séries são cruciais na resolução de equações diferenciais e no desenvolvimento de algoritmos para computação científica.

## Convergência

A convergência das séries de Taylor depende do ponto $a$ escolhido e da função $f(x)$. Para muitas funções, a série converge para a função em um intervalo ao redor de $x = a$, conhecido como o intervalo de convergência.

### Raio De Convergência

Para determinar o raio de convergência de uma série de Taylor, podemos usar o teste do raio de Cauchy (ou teste da razão). O raio de convergência $R$ é dado pela fórmula:

$$
 R = \lim_{n \to \infty} \left| \frac{a_n}{a_{n+1}} \right| 
$$

onde $a_n = \frac{f^{(n)}(a)}{n!}(x-a)^n$ são os coeficientes da série de Taylor.

Vamos aplicar esse método aos exemplos fornecidos:

### Exemplo 1: Função Exponencial $e^x$

A série de Maclaurin (série de Taylor em torno do ponto $x = 0$) para a função exponencial é:

$$
 e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} 
$$

Neste caso, os coeficientes são $a_n = \frac{1}{n!}$.

Para encontrar o raio de convergência, usamos:

$$
 R = \lim_{n \to \infty} \left| \frac{a_n}{a_{n+1}} \right| = \lim_{n \to \infty} \left| \frac{\frac{1}{n!}}{\frac{1}{(n+1)!}} \right| = \lim_{n \to \infty} \left| \frac{(n+1)!}{n!} \right| = \lim_{n \to \infty} (n+1) = \infty 
$$

Portanto, o raio de convergência é $R = \infty$, o que significa que a série converge para toda $x$.

### Exemplo 2: Função Cosseno $\cos(x)$

A série de Taylor em torno do ponto $x = 0$ para a função cosseno é:

$$
 \cos(x) = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n}}{(2n)!} 
$$

Neste caso, os coeficientes são $a_n = (-1)^n \frac{1}{(2n)!}$.

Para encontrar o raio de convergência, usamos:

$$
 R = \lim_{n \to \infty} \left| \frac{a_n}{a_{n+1}} \right| = \lim_{n \to \infty} \left| \frac{(-1)^n \frac{1}{(2n)!}}{(-1)^{n+1} \frac{1}{(2(n+1))!}} \right| = \lim_{n \to \infty} \left| \frac{(2(n+1))!}{(2n)!} \cdot \frac{1}{-1} \right| = \lim_{n \to \infty} (2n+2)(2n+1) = \infty 
$$

Portanto, o raio de convergência é $R = \infty$, o que significa que a série converge para toda $x$.

### Exemplo 3: Função Seno $\sin(x)$

A série de Taylor em torno do ponto $x = 0$ para a função seno é:

$$
 \sin(x) = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n+1}}{(2n+1)!} 
$$

Neste caso, os coeficientes são $a_n = (-1)^n \frac{1}{(2n+1)!}$.

Para encontrar o raio de convergência, usamos:

$$
 R = \lim_{n \to \infty} \left| \frac{a_n}{a_{n+1}} \right| = \lim_{n \to \infty} \left| \frac{(-1)^n \frac{1}{(2n+1)!}}{(-1)^{n+1} \frac{1}{(2(n+1)+1)!}} \right| = \lim_{n \to \infty} \left| \frac{(2(n+1)+1)!}{(2n+1)!} \cdot \frac{1}{-1} \right| = \lim_{n \to \infty} (2n+3)(2n+2) = \infty 
$$

Portanto, o raio de convergência é $R = \infty$, o que significa que a série converge para toda $x$.
