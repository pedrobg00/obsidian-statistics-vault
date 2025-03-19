As séries são uma parte fundamental do cálculo que nos permitem estudar somas infinitas de termos. Elas são ferramentas matemáticas poderosas que aparecem em diversos contextos, desde problemas práticos até aplicações teóricas avançadas.

## O Que São Séries?

Uma série é a soma de uma sequência infinita de números. Matematicamente, é representada como:

$$
 \sum_{n=1}^{\infty} a_n = a_1 + a_2 + a_3 + … 
$$

## Tipos Principais De Séries

- **Séries Geométricas:** São séries onde cada termo é multiplicado por uma razão constante
- **Séries Aritméticas:** São séries onde a diferença entre termos consecutivos é constante
- **Séries de Potência:** São séries que envolvem potências de uma variável

## Conceitos Fundamentais

- **Convergência:** Uma série converge quando a soma de seus termos se aproxima de um valor finito
- **Divergência:** Uma série diverge quando a soma de seus termos não se aproxima de um valor finito

O estudo das séries é essencial para compreender diversos fenômenos matemáticos e tem aplicações em física, engenharia e outras áreas das ciências.

## Séries Geométricas

Uma série geométrica é caracterizada por ter uma razão constante (r) entre termos consecutivos. A forma geral de uma série geométrica é:

$$
 a + ar + ar^2 + ar^3 + … = \sum_{n=0}^{\infty} ar^n 
$$

Onde 'a' é o primeiro termo e 'r' é a razão da série. A convergência de uma série geométrica depende diretamente do valor absoluto da razão |r|.

### Convergência De Séries Geométricas

Uma série geométrica pode convergir ou divergir dependendo do valor da razão r:

- **Quando |r| < 1:** A série converge para a soma:
$$
 \sum_{n=0}^{\infty} ar^n = \frac{a}{1-r} 
$$
- **Quando |r| ≥ 1:** A série diverge (não tem soma definida)

Exemplo: Para a série geométrica com a = 2 e r = 1/2:

$$
 2 + 1 + \frac{1}{2} + \frac{1}{4} + … 
$$

Como |r| = |1/2| = 0.5 < 1, a série converge e podemos calcular sua soma:

$$
 \frac{2}{1-\frac{1}{2}} = \frac{2}{\frac{1}{2}} = 4 
$$

### Casos Especiais

- **r = 1:** A série diverge para +∞ (se a > 0)
- **r = -1:** A série oscila e diverge
- **r = 0:** A série tem apenas um termo (a) e converge trivialmente

## Soma De Séries Por Sequências Parciais

[[Soma de Séries por Sequências Parciais]]
