A **fatoração LU** (lower-upper) é um método matemático utilizado para decompor uma matriz quadrada $A$ em duas matrizes, uma triangular inferior $L$ e uma triangular superior $U$, tal que:

$$ A = L U $$

## Exemplos De Matrizes Triangulares Inferior E Superior

- **Matriz Triangular Inferior $L$:**

  $$ L = \begin{pmatrix}
  l_{11} & 0 & 0 \\
  l_{21} & l_{22} & 0 \\
  l_{31} & l_{32} & l_{33}
  \end{pmatrix} $$
  

- **Matriz Triangular Superior $U$:**

  $$ U = \begin{pmatrix}
  u_{11} & u_{12} & u_{13} \\
  0 & u_{22} & u_{23} \\
  0 & 0 & u_{33}
  \end{pmatrix} $$



## Exemplo De Decomposição Lu

Considere a matriz $A$:

$$ A = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix} $$

A decomposição LU resulta em:

- **Matriz Triangular Inferior $L$:**
  $$ L = \begin{pmatrix}
  1 & 0 & 0 \\
  4 & 1 & 0 \\
  7 & -2 & 1
  \end{pmatrix} $$

- **Matriz Triangular Superior $U$:**
  $$ U = \begin{pmatrix}
  1 & 2 & 3 \\
  0 & -3 & -6 \\
  0 & 0 & 0
  \end{pmatrix} $$

### Utilizações Da Fatoração Lu Para Resolução De Sistemas Lineares

A fatoração LU é especialmente útil na resolução de sistemas lineares, pois:

1. **Resolução do Sistema $Ax = b$:**
   - Decomponha a matriz $A$ em $L$ e $U$.
   - Resolva o sistema triangular inferior $Ly = b$ para obter $y$.
   - Resolva o sistema triangular superior $Ux = y$ para obter $x$.

2. **Eficiência Computacional:**
   - A decomposição LU é computacionalmente eficiente, especialmente quando a matriz $A$ é grande e estática (não muda frequentemente).
   - O tempo de resolução do sistema linear após a decomposição é proporcional ao número de operações necessárias para resolver os sistemas triangulares.

3. **Aplicações em Engenharia e Ciência:**
   - Solução de problemas de equilíbrio estrutural.
   - Simulação de fluidos.
   - Modelagem de sistemas dinâmicos.

4. **Estabilidade Numérica:**
   - A fatoração LU pode ser estabilizada com pivoteamento parcial para evitar divisões por zero e minimizar erros numéricos.

### Exemplo De Resolução De Um Sistema Linear

Considere o sistema linear:

$$ \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix} x = \begin{pmatrix}
10 \\
11 \\
12
\end{pmatrix} $$

Após a decomposição LU, resolvemos os sistemas triangulares:

- **Resolução de $Ly = b$:**
  $$ L = \begin{pmatrix}
  1 & 0 & 0 \\
  4 & 1 & 0 \\
  7 & -2 & 1
  \end{pmatrix}, \quad y = \begin{pmatrix}
  10 \\
  6 \\
  3
  \end{pmatrix} $$

- **Resolução de $Ux = y$:**
  $$ U = \begin{pmatrix}
  1 & 2 & 3 \\
  0 & -3 & -6 \\
  0 & 0 & 0
  \end{pmatrix}, \quad x = \begin{pmatrix}
  1 \\
  -1 \\
  0
  \end{pmatrix} $$

Portanto, a solução do sistema é $x = \begin{pmatrix} 1 \\ -1 \\ 0 \end{pmatrix}$.

