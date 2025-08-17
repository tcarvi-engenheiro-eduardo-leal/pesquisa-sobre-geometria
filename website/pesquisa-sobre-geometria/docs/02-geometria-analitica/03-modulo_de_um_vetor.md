# Módulo de um Vetor

O **módulo de um vetor** (também chamado de **norma** ou **comprimento**) é uma medida da magnitude desse vetor em um espaço vetorial. Formalmente, o módulo de um vetor $ \vec{v} $ em $ \mathbb{R}^n $ é definido como:

$$ \| \vec{v} \| = \sqrt{v_1^2 + v_2^2 + \dots + v_n^2} $$

onde $ \vec{v} = (v_1, v_2, \dots, v_n) $ representa as componentes do vetor.

## Propriedades do Módulo de um Vetor

1. **Não-negatividade**:  
   $ \| \vec{v} \| \geq 0 $, e  
   $ \| \vec{v} \| = 0 $ se e somente se $ \vec{v} = \vec{0} $

2. **Homogeneidade**:  
   Para qualquer escalar $ \alpha \in \mathbb{R} $,  
   $ \| \alpha \vec{v} \| = |\alpha| \cdot \| \vec{v} \| $

3. **Desigualdade Triangular**:  
   Para quaisquer vetores $ \vec{u} $ e $ \vec{v} $,  
   $ \| \vec{u} + \vec{v} \| \leq \| \vec{u} \| + \| \vec{v} \| $

## Interpretação Geométrica

Em $ \mathbb{R}^2 $ ou $ \mathbb{R}^3 $, o módulo de um vetor $ \vec{v} $ representa a distância euclidiana da origem até o ponto definido por $ \vec{v} $.

- **Em $ \mathbb{R}^2 $**:  
  Se $ \vec{v} = (x, y) $, então:  
  $ \| \vec{v} \| = \sqrt{x^2 + y^2} $.

- **Em $ \mathbb{R}^3 $**:  
  Se $ \vec{v} = (x, y, z) $, então:  
  $ \| \vec{v} \| = \sqrt{x^2 + y^2 + z^2} $.

## Cálculo do Módulo

Dado um vetor $ \vec{v} = (3, 4) $ em $ \mathbb{R}^2 $, seu módulo é:  
$
\| \vec{v} \| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5.
$

## Relação com o Produto Escalar

O módulo de um vetor também pode ser expresso em termos do **produto escalar**:  
$
\| \vec{v} \| = \sqrt{ \vec{v} \cdot \vec{v} }.
$

## Casos Especiais

- **Vetor Unitário**: Um vetor $ \vec{u} $ é dito **unitário** se $ \| \vec{u} \| = 1 $.
- **Normalização**: Qualquer vetor não nulo $ \vec{v} $ pode ser normalizado dividindo-o por seu módulo:  
  $
  \vec{u} = \frac{\vec{v}}{\| \vec{v} \|}.
  $
