## Introdução Ao Método De Eliminação De Gauss

O Método de Eliminação de Gauss é uma técnica fundamental utilizada para resolver sistemas lineares de equações. Este método consiste em transformar um sistema linear em uma forma triangular superior, facilitando a resolução do mesmo através da substituição retroativa.

### Passos Básicos Do Método

1. **Forma Triangular Superior:**
   - O objetivo é transformar o sistema linear original em uma matriz triangular superior.
   - Isso é feito através de operações elementares nas linhas do sistema, sem alterar a solução do mesmo.

2. **Operações Elementares:**
   - Adição múltipla de uma linha à outra.
   - Troca de duas linhas entre si.
   - Multiplicação de uma linha por um escalar não nulo.

3. **Etapa de Eliminação:**
   - Para cada coluna, a ideia é eliminar os elementos abaixo da diagonal principal.
   - Isso é feito multiplicando a primeira equação pelo fator adequado e subtraindo-a das demais equações correspondentes.

4. **Etapa de Substituição Retroativa:**
   - Após obter a forma triangular superior, o sistema pode ser resolvido facilmente através da substituição retroativa.
   - Começa pela última equação e resolve para a última variável, depois usa esse valor na penúltima equação, e assim por diante.

### Exemplo

Considere o seguinte sistema linear:

$$


\begin{cases}

2x + 3y - z = 1 \\

-3x - 5y + 2z = -1 \\

5x + y - 9z = 6

\end{cases}


$$

**Passo 1: Eliminação**
- Transformar o sistema em uma matriz:
  $$

  \left[\begin{array}{ccc|c}
  2 & 3 & -1 & 1 \\
  -3 & -5 & 2 & -1 \\
  5 & 1 & -9 & 6
  \end{array}\right]
  
$$

- Eliminar $x$ da segunda e terceira equações:
  $$

  R_2 = R_2 + \frac{3}{2}R_1, \quad R_3 = R_3 - \frac{5}{2}R_1

$$
  Resultando em:
  $$

  \left[\begin{array}{ccc|c}
  2 & 3 & -1 & 1 \\
  0 & \frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
  0 & -\frac{13}{2} & -\frac{13}{2} & \frac{7}{2}
  \end{array}\right]

$$

- Eliminar $y$ da terceira equação:
  $$

  R_3 = R_3 + 13R_2

$$
  Resultando em:
  $$

  \left[\begin{array}{ccc|c}
  2 & 3 & -1 & 1 \\
  0 & \frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\
  0 & 0 & -6 & 7
  \end{array}\right]

$$

**Passo 2: Substituição Retroativa**
- Resolvendo a última equação:
  $$

  -6z = 7 \implies z = -\frac{7}{6}

$$

- Usando $z$ na segunda equação:
  $$

  \frac{1}{2}y + \frac{1}{2}\left(-\frac{7}{6}\right) = \frac{1}{2} \implies y - \frac{7}{12} = \frac{1}{2} \implies y = \frac{5}{6}

$$

- Usando $y$ e $z$ na primeira equação:
  $$

  2x + 3\left(\frac{5}{6}\right) - \left(-\frac{7}{6}\right) = 1 \implies 2x + \frac{15}{6} + \frac{7}{6} = 1 \implies 2x + 4 = 1 \implies x = -\frac{3}{2}

$$

Portanto, a solução é $x = -\frac{3}{2}$, $y = \frac{5}{6}$, e $z = -\frac{7}{6}$.

