# Triângulo

Um triângulo é uma figura geométrica plana definida por três pontos não colineares e pelos três segmentos de reta que os conectam. Formalmente, podemos descrevê-lo da seguinte maneira:

## Definição Formal

Sejam **A**, **B** e **C** três pontos distintos em um plano euclidiano $\mathbb{R}^2$, tais que não são colineares (não pertencem a uma mesma reta). O **triângulo** $\triangle ABC$ é o conjunto formado pela união dos três segmentos de reta $\overline{AB}$, $\overline{BC}$ e $\overline{CA}$:

$$
\triangle ABC = \overline{AB} \cup \overline{BC} \cup \overline{CA}
$$

onde:
- $\overline{AB}$ é o segmento de reta que liga **A** a **B**, dado por:
  $$
  \overline{AB} = \{ P \in \mathbb{R}^2 \mid P = A + t(B - A), \ t \in [0,1] \}
  $$
- Analogamente para $\overline{BC}$ e $\overline{CA}$.

## Elementos do Triângulo
1. **Vértices**: Os pontos **A**, **B** e **C**.
2. **Lados**: Os segmentos $\overline{AB}$, $\overline{BC}$ e $\overline{CA}$.
3. **Ângulos internos**: Os ângulos formados entre os lados, denotados por $\angle BAC$, $\angle ABC$ e $\angle ACB$, com:
   $$
   \angle BAC + \angle ABC + \angle ACB = 180^\circ
   $$

## Área do Triângulo
- A área $\mathcal{A}$ do triângulo pode ser calculada por:
$$
\mathcal{A} = \frac{1}{2} \| \vec{AB} \times \vec{AC} \|
$$
    - onde: 
        - $\vec{AB} = B - A$ ,
        - $\vec{AC} = C - A$  e 
        - $\times$  denota o produto vetorial em  $\mathbb{R}^2$  (equivalente ao determinante da matriz formada pelos vetores).

## Condição de Existência (Desigualdade Triangular)
- Para que três pontos formem um triângulo, a soma de quaisquer dois lados deve ser maior que o terceiro:
$$
\|B - A\| + \|C - B\| > \|C - A\| \\
\|A - B\| + \|C - A\| > \|B - C\| \\
\|B - C\| + \|C - A\| > \|A - B\|
$$