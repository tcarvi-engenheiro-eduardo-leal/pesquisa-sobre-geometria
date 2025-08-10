# Produto Misto
- O produto misto é uma operação que combina três vetores do espaço tridimensional (ℝ³) e resulta em um escalar (um número real).
- Ele envolve dois passos:
    - Produto vetorial entre dois vetores.
    - Produto escalar do resultado com um terceiro vetor.

## Definição Formal
- Dados três vetores: $\vec{u}$, $\vec{v}$ e $\vec{w}$, em $\R^{3}$, o produto misto é definido por:  
    - $ [\vec{u}, \vec{v}, \vec{w}]  = \vec{u} \cdot ( \vec{v} \times \vec{w} ) $.  
- Ou, equivalentemente, o produto misto é igual ao determinante da matriz formada pelos vetores:
$$
[\vec{u}, \vec{v}, \vec{w}] = \det \begin{pmatrix}
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3 \\
w_1 & w_2 & w_3 \\
\end{pmatrix}
$$

## Interpretação Geométrica
- O valor absoluto do produto misto representa o volume do paralelepípedo formado pelos vetores $\vec{u}$, $\vec{v}$ e $\vec{w}$:
    - $ \text{Volume} = \left| \vec{u} \cdot (\vec{v} \times \vec{w}) \right| $
- Significado dos sinais do Produto Misto:
    - Se o produto misto é igual a zero, os vetores são coplanares.
    - Se o produto misto é positivo, a tripla $(\vec{u}, \vec{v}, \vec{w})$ segue a regra da mão direita.
    - Se o produto misto é negativo, a tripla $(\vec{u}, \vec{v}, \vec{w})$ segue a regra da mão esquerda.

## Propriedades do Produto Misto
- Propriedade da permutação cíclica:
    - $ \vec{u} \cdot (\vec{v} \times \vec{w}) = \vec{w} \cdot (\vec{u} \times \vec{v}) = \vec{v} \cdot (\vec{w} \times \vec{u})$
    - Em notação de produto misto:
        - $ [\vec{u}, \vec{v}, \vec{w}] = [\vec{w}, \vec{u}, \vec{v}] = [\vec{v}, \vec{w}, \vec{u}]$
- Propriedade de Antissimetria:
    - Para quaisquer vetores $\vec{u}$, $\vec{v}$, $\vec{w}$ $\in \R^3$, a troca de dois vetores inverte o sinal do produto misto:
        - $ \vec{u} \cdot (\vec{v} \times \vec{w}) = - \vec{u} \cdot (\vec{w} \times \vec{v}) $
            - Em notação de produto misto:
                - $[\vec{u}, \vec{v}, \vec{w}] = -[\vec{u}, \vec{w}, \vec{v}]$
    - A antissimetria reflete o comportamento do determinante ante trocas de linhas (ou colunas).
        - Como o produto misto é equivalente a um determinante, trocar dois vetores (linhas) inverte o sinal do resultado. Não altera o valor absoluto (mas sim a orientação do sistema). Se a troca ocorre duas vezes, retorna-se ao sinal original. 
- Linearidade
    - O produto misto possui a propriedade de linearidade em relação a cada um de seus vetores componentes.
    - Isso significa que o Produto Misto é linear em cada argumento da formulação de seu produto, ou seja, satisfaz as propriedades de aditividade e homogeneidade, quando decompomos cada argumento em uma soma de vetores componentes.
    - Formulação da propriedade de Linearidade:
        - Considere o cada $\vec{vetor}$ pode ser descrito por 2 componentes $\vec{vertor_1}$ e $\vec{vetor_2}$ multiplicados, cada um, por algum valor real.
        - Assim, considerando:
            - Vetores componentes $\vec{vetor_1}, \vec{vertor_2}, \vec{u}, \vec{v} \: e \: \vec{w} \in \R^3$ e
            - Escalares $\alpha, \beta \in \R$
        - Formulamos que:
            - $ (\alpha \vec{u_1} + \beta \vec{u_2}) \cdot (\vec{v} \times \vec{w})=\alpha(\vec{u_1} \cdot (\vec{v} \times \vec{w})) + \beta(\vec{u_2} \cdot (\vec{v} \times \vec{w})) $
            - $ \vec{u} \cdot ((\alpha \vec{v}_1 + \beta \vec{v}_2) \times \vec{w}) = \alpha (\vec{u} \cdot (\vec{v}_1 \times \vec{w})) + \beta (\vec{u} \cdot (\vec{v}_2 \times \vec{w})) $
            - $ \vec{u} \cdot (\vec{v} \times (\alpha \vec{w}_1 + \beta \vec{w}_2)) = \alpha (\vec{u} \cdot (\vec{v} \times \vec{w}_1)) + \beta (\vec{u} \cdot (\vec{v} \times \vec{w}_2)) $
        - Em resumo, formulamos a multilinearidade, devido a linearidade nos 3 vetores:
            - $ [\alpha_1 \vec{u}_1 + \alpha_2 \vec{u}_2, \beta_1 \vec{v}_1 + \beta_2 \vec{v}_2, \gamma_1 \vec{w}_1 + \gamma_2 \vec{w}_2] = \sum_{i,j,k} \alpha_i \beta_j \gamma_k [\vec{u}_i, \vec{v}_j, \vec{w}_k] $


## Aplicações
- Em Geometria Analítica:
    - Usado para verifica coplanaridade de pontos.
    - Considera-se que cada ponto, (A, B e C), é um vetor.
    - Se o produto misto $[\vec{A}, \vec{B}, \vec{C}] = 0$, os vetores e os pontos estão no mesmo plano.
        - A única possibilidade dos 3 vetores não poderem ser incluídos no mesmo plano é se os três forem colineares. Neste caso, o produto misto será diferente de zero e será impossível determinar um plano para os três pontos.
- Em Física:
    - Cálculo de torque:
    - Cálculo de momento angular:
- Em Engenharia:
    - Análise de tensões em materiais:
