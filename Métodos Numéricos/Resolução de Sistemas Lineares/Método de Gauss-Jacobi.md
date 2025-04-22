O Método de Gauss-Jacobi é um algoritmo iterativo utilizado para resolver sistemas lineares de equações do tipo $Ax = b$, onde $A$ é uma matriz quadrada, $x$ e $b$ são vetores. Este método é particularmente útil quando a matriz $A$ possui certas propriedades que facilitam sua aplicação.

## Formulando O Problema

Considere um sistema linear de equações representado por:

$$
\begin{align*}
a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n &= b_1 \\
a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n &= b_2 \\
&\vdots \\
a_{n1}x_1 + a_{n2}x_2 + \cdots + a_{nn}x_n &= b_n
\end{align*}
$$

Podemos expressar este sistema em forma matricial como $Ax = b$, onde:

- $A$ é uma matriz $n \times n$,
- $x$ é um vetor coluna de incógnitas,
- $b$ é um vetor coluna dos termos independentes.

## Aplicação Do Método

O método de Gauss-Jacobi consiste em decompor a matriz $A$ em suas partes diagonal, triangular inferior e triangular superior. Especificamente, podemos escrever:

$$
A = D + L + U,
$$

onde $D$ é a matriz diagonal formada pelos elementos da diagonal principal de $A$, $L$ é a matriz triangular inferior (com zeros na diagonal) e $U$ é a matriz triangular superior (também com zeros na diagonal).

Assim, o sistema original pode ser reescrito como:

$$
Dx = -Lx - Ux + b.
$$

Isolando $x$, obtemos:

$$
x^{(k+1)} = D^{-1}(-Lx^{(k)} - Ux^{(k)} + b),
$$

onde $x^{(k)}$ representa a aproximação do vetor solução no $k$-ésimo passo.

## Exemplo

Considere o sistema linear:

$$
\begin{align*}
2x_1 + x_2 &= 8 \\
x_1 + 3x_2 &= 10
\end{align*}
$$

Em forma matricial, temos $A = \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix}$, $b = \begin{pmatrix} 8 \\ 10 \end{pmatrix}$.

Aplicando o método de Gauss-Jacobi:

$$
x_1^{(k+1)} = \frac{1}{2}(8 - x_2^{(k)}) \\
x_2^{(k+1)} = \frac{1}{3}(10 - x_1^{(k)})
$$

## Convergência E Considerações Finais

A convergência do método de Gauss-Jacobi depende das propriedades da matriz $A$. Especificamente, o método converge se a matriz $A$ for diagonalmente dominante ou se todas as entradas abaixo da diagonal principal forem negativas.

Embora eficiente em muitos casos, o método de Gauss-Jacobi pode ser mais lento que outros métodos iterativos como o de Gauss-Seidel. No entanto, sua simplicidade e facilidade de implementação tornam-no uma ferramenta valiosa em diversas aplicações práticas.
