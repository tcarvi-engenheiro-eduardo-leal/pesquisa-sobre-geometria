# Vetor
- Em **Geometria Analítica**, um vetor é um objeto matemático que possui **magnitude** (comprimento), **direção** e **sentido**. 

## Vetor (Definição na Algebra)
- Seja $ {\R}^n $ o espaço euclidiano n-dimensional. 
    - Um vetor $ v $ em $ {\R}^n $ é uma n-upla ordenada de números reais:  
        - $ \vec{\upsilon} = ( \vec{{\upsilon}_1}, \vec{{\upsilon}_2}, ... , \vec{{\upsilon}_n} ) $, onde $ \vec{{\upsilon}_i} \in \R $, $ i = 1, 2, ..., n $
    - Um vetor também pode ser representado por uma matriz coluna: 
$$
\vec{\upsilon} = \begin{pmatrix}
   {\upsilon}_1 \\
   {\upsilon}_2 \\
   ...          \\
   {\upsilon}_n \\
\end{pmatrix}
$$
  
---  
  
## Vetor (Definição na Geometria Analítica)
- Geometricamente, um vetor é uma **classe de equivalência de segmentos orientados** (setas) com mesma direção, sentido e comprimento.  
- **Definição de Vetor como Segmento Orientado:**
    - Sejam A e B pontos no espaço $ {\R}^n $. O **vetor** $ \overrightarrow{AB} $ é o segmento orientado que:
        - Tem **origem** em A.
        - Tem **extremidade** em B.
        - Seu **comprimento** é a distância euclidiana d(A, B).
        - Sua **direção** é a da reta que passa por A e B.
        - Seu **sentido** é de A para B.

- **Definição de Vetor como Classe de Equivalência:**
    - Dois segmentos orientados $ \overrightarrow{AB} $  e $ \overrightarrow{CD} $  representam o **mesmo vetor** se e somente se:
        - $ B - A = D - C
        - Ou seja, têm as mesmas componentes.
            - Isso significa que vetores **não têm posição fixa**; apenas direção, sentido e magnitude importam.

## Versor
- Um vetor com magnitude igual a 1 unidade de medida.
- Exemplos:
    - Versor $ \vec{i} = (1, 0, 0) $
    - Versor $ \vec{j} = (0, 1, 0) $
    - Versor $ \vec{k} = (0, 0, 1) $
- Versor gerado a partir de um vetor qualquer $ \vec{AB} $:
    - Versor = $ \frac{ \vec{AB}}{|\vec{AB}|} $
    - Versor = $ ( \frac{X_B - X_A}{|\vec{AB}|}, \frac{Y_B - Y_A}{|\vec{AB}|}) $

## Inclinação de Um Vetor
- Tangente do ângulo do vetor, considerndo o ângulo como com abertura, para o lado direito ou para cima, do cruzamento com o eixo x.
- Inclinação = Tangente do ângulo = $ \frac{ Y_B - Y_A }{ X_B - X_A } $

 
