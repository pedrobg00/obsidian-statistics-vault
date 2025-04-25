Derivadas parciais permitem a análise de funções com múltiplas variáveis, permitindo estudar como uma função muda quando apenas uma das suas variáveis é alterada, mantendo as outras constantes.

Consideremos uma função $f(x, y)$ que depende de duas variáveis, $x$ e $y$. A derivada parcial de $f$ com respeito a $x$, denotada por $\frac{\partial f}{\partial x}$, representa o ritmo de mudança da função em relação à variável $x$, considerando que $y$ é mantido constante. Analogamente, a derivada parcial com respeito a $y$, denotada por $\frac{\partial f}{\partial y}$, mede como a função muda quando $y$ varia e $x$ permanece inalterado.

Por exemplo, considere a função $f(x, y) = x^2 + 3xy - 4y^2$. A derivada parcial de $f$ com respeito a $x$ é:

$$
\frac{\partial f}{\partial x} = 2x + 3y.
$$

Aqui, observamos que a variável $y$ é tratada como uma constante durante o cálculo da derivada parcial.

Analogamente, a derivada parcial de $f$ com respeito a $y$ é:

$$
\frac{\partial f}{\partial y} = 3x - 8y.
$$

Neste caso, $x$ é considerado constante durante o cálculo da derivada parcial.

## Regra Geral

Quando você deriva uma função $f(x, y, z, \ldots)$ em relação a uma variável (por exemplo, $x$), **as outras são tratadas como constantes**.

---

## **Exemplo 1: Função Simples Com Duas variáveis**

Seja:

	$f(x, y) = x^2 y + 4y^3$

### **Derivada Parcial Em Relação a** $x$

$$\frac{\partial f}{\partial x} = \frac{\partial}{\partial x} (x^2 y + 4y^3)$$

- y é constante, então:
- $x^2 y \rightarrow \text{deriva como } 2xy$
- $4y^3 \rightarrow \text{deriva como } 0$ (constante em x)

**Resultado:**

$$\frac{\partial f}{\partial x} = 2xy$$

### **Derivada Parcial Em Relação a** $y$

$$\frac{\partial f}{\partial y} = \frac{\partial}{\partial y} (x^2 y + 4y^3)$$

- $x^2$ é constante agora
- $x^2 y \rightarrow x^2$
- $4y^3 \rightarrow 12y^2$

**Resultado:**

$$\frac{\partial f}{\partial y} = x^2 + 12y^2$$
