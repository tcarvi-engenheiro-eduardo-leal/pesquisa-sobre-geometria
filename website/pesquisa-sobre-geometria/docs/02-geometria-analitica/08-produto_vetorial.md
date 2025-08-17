# Produto Vetorial

## Definição Formal
- Dados dois vetores $ \vec{u} = (u_1, u_2, u_3) $ e $ \vec{v} = (v_1, v_2, v_3) $ em $ {\R}^3 $,  
o produto vetorial $ \vec{u} \times \vec{v} $ é definido como:  
$  \vec{u} \times \vec{v} =  \begin{vmatrix} \vec{i} & \vec{j} & \vec{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \\ \end{vmatrix} $  
- Onde $ \vec{i}, \vec{j}, \vec{k} $ são os vetores unitários nas direções dos eixos x, y e z, respectivamente.

## Propriedades do Produto Vetorial
- **Direção e sentido**:
    - O vetor resultante $ \vec{u} \times \vec{v} $ é perpendicular tanto a $ \vec{u} $ quanto a $ \vec{v} $ , seguindo a **regra da mão direita**:
        - Aponte os dedos na direção do primeiro vetor  $ \vec{u} $.
        - Dobre-os na direção do segundo vetor $ \vec{v} $.
        - O polegar apontará na direção de $ \vec{u} \times \vec{v} $.

- ***Magnitude (Norma)***:
    - $ \begin{Vmatrix} \vec{u} \times \vec{v} \end{Vmatrix} = \begin{Vmatrix} \vec{u} \end{Vmatrix} \begin{Vmatrix} \vec{v} \end{Vmatrix} \sin \theta $
        - Onde θ é o ângulo entre $ \vec{u} $ e $ \vec{v} $.
        - A Magnitude (Norma) do produto vetorial é igual à área do paralelogramo formado por $ \vec{u} $ e $ \vec{v} $.

- **Anticomutatividade**:  
    - $ \vec{u} \times \vec{v} = -(\vec{v} \times \vec{u}) $

- **Distributividade**:  
    - $ \vec{u} \times (\vec{v} + \vec{w}) = \vec{u} \times \vec{v} + \vec{u} \times \vec{w} $

- **Produto Vetorial com vetor nulo**:  
    - $ \vec{u} \times \vec{0} = \vec{0} \times \vec{u} = \vec{0} $

- **Produto Vetorial de vetores paralelos**:
    - Se $ \vec{u} $ e $ \vec{v} $ são paralelos (θ = 0° ou 180°), então:  
        - $ \vec{u} \times \vec{v} = \vec{0} $

## Aplicações do Produto Vetorial
- **Cálculo de Áreas**:
    - Determinação de áreas de paralelogramos.
        - Tendo dois vetores, A e B. A área do paralelogramo formado pelos dois vetores é numericamente igual ao módulo do produto vetorial dos dois vetores.
    - Determinação de áreas de triângulos.
        - Tendo dois vetores, A e B. A área do triángulo formado pelos dois vetores é numericamente igual à metade da área do paralelogramo formado por estes mesmos dois vetores.
- **Física**:
    - Cálculo de torque (τ = **r × F**),
    - Cálculo de momento angular (**L = r × p**)
    - Cálculo de força magnética (**F = q v × B**)
- **Computação gráfica**:
    - Cálculo de normais a superfícies para iluminação e renderização 3D.
