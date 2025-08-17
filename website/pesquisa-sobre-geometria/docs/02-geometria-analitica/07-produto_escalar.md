# Produto Escalar

## Representação:
- $ \Braket{ \vec{u}, \vec{v} } $
- $ \vec{u} ⋅ \vec{v}$
## Definição:
- Dados dois vetores $ \vec{u} = (u_1, u_2, ..., u_n) $ e $ \vec{v} = (v_1, v_2, ..., v_n) $ em $ {\R}^n $, o produto escalar é definido por:
    - $ \vec{u} ⋅ \vec{v} = \displaystyle\sum_{i=1}^{n}{u_{i}.v_{i}} = u_{1}.v_{1} + u_{2}.v_{2} + ... + u_{n}.v_{n} $

- Caso Particular em $ {\R}^2 $: 
    - $ \vec{u} ⋅ \vec{v} = u_{1}.v_{1} + u_{2}.v_{2} $ 

- Caso Particular em $ {\R}^3 $
    - - $ \vec{u} ⋅ \vec{v} = u_{1}.v_{1} + u_{2}.v_{2} + u_{3}.v_{3} $ 

- Definição adicional:
    - Produto das magnitudes de dois vetores multiplicado pelo cosseno do ângulo entre os vetores.
        - $ \vec{u} ⋅ \vec{v} = ||\vec{u}|| \: ||\vec{v}|| \: cos{\theta} $ 


## Características Importantes
- Sobre vetores perpendiculares:
    - ($\theta$ = 90°) →  $ \vec{u} ⋅ \vec{v} = 0 $. 
- Sobre vetores paralelos:
    - ($\theta$ = 0° ou 180°) → $ \vec{u} ⋅ \vec{v} = \pm \: ||\vec{u}|| \: ||\vec{v}|| $. 
- Sobre o sinal do produto escalar:
    - Positivo → Ângulo agudo entre os vetores (θ < 90°)
    - Negativo → Ângulo obtuso entre os vetores (θ > 90°)

## Propriedades do Produto Escalar
- Comutatividade:
    - $ \vec{u} ⋅ \vec{v} = \vec{v} ⋅ \vec{u} $
- Distributividade:
    - $ \vec{u} ⋅ (\vec{v} + \vec{w}) = \vec{u} ⋅ \vec{v} + \vec{u} ⋅ \vec{w} $
- Multiplicação por escalar:
    - $ (k \vec{u}) ⋅ \vec{v} = k (\vec{u} ⋅ \vec{v}) $
- Norma (módulo) de um vetor:
    - $ ||\vec{u}|| = \sqrt{ \vec{u} ⋅ \vec{u} }$
​

## Aplicações na Física:
- Trabalho realizado por uma força 
    - $ \vec{W} = \vec{F} \sdot \vec{d} = ||\vec{F}|| \: ||\vec{d}|| \: cos{\theta} $
- Fluxo de campos vetoriais.
    - $ \Phi = \iint_S \vec{F} \cdot d\vec{S} $
    - "Para uma superfície S, o **Fluxo de um Campo Vetorial** ($\Phi$) é igual à *integral dupla calculada sobre a superfície S* ($\iint_S$), do produto escalar entre **Vetor Campo Vetorial** $\vec{F}$ e **Vetor de Área Infinitesimal** $ d\vec{S} $".