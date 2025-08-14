# Distância Entre Dois Pontos

## Distância entre dois pontos, no espaço bidimensional
- $ d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2} $
    - Sendo:
        - $ d $ =: distância entre pontos $ P_1 $ e $ P_2 $
        - $ x_2 $ =: Posição, no eixo x, do ponto $ P_2 $
        - $ x_1 $ =: Posição, no eixo x, do ponto $ P_1 $
        - $ y_2 $ =: Posição, no eixo y, do ponto $ P_2 $
        - $ y_1 $ =: Posição, no eixo y, do ponto $ P_1 $

## Distância entre dois pontos, no espaço tridimensional
- $ d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2 + (z_2 - z_1)^2 } $
    - Sendo:
        - $ d $ =: distância entre pontos $ P_1 $ e $ P_2 $
        - $ x_2 $ =: Posição, no eixo x, do ponto $ P_2 $
        - $ x_1 $ =: Posição, no eixo x, do ponto $ P_1 $
        - $ y_2 $ =: Posição, no eixo y, do ponto $ P_2 $
        - $ y_1 $ =: Posição, no eixo y, do ponto $ P_1 $
        - $ z_2 $ =: Posição, no eixo z, do ponto $ P_2 $
        - $ z_1 $ =: Posição, no eixo z, do ponto $ P_1 $

## Distância entre dois pontos, no espaço 4D, com dados normalizados e ponderados
- Como humanos, não percebemos a distância no espaco 4D. 
    - Mas o significado é simples:
        - Supomos 3 objetos de cores diferentes, no espaco 3D.
        - Desejamos uma métrica para saber a aproximação (distância) de cada dupla destes objetos.
        - E desejamos comparar a medida de distância entre duplas diferentes de objetos.
        - Basta usar a mesma fórmula da distância de dois pontos, mas acrescentando uma coordenada, que chamarei por w.
    - Então, para ter uma medida de distância entre os dois objetos, calculamos:
        - $ d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2 + (z_2 - z_1)^2 + (w_2 - w_1)} $
            - Sendo:
                - $ d $ =: distância entre pontos $ P_1 $ e $ P_2 $
                - $ x_2 $ =: Posição, no eixo x, do ponto $ P_2 $
                - $ x_1 $ =: Posição, no eixo x, do ponto $ P_1 $
                - $ y_2 $ =: Posição, no eixo y, do ponto $ P_2 $
                - $ y_1 $ =: Posição, no eixo y, do ponto $ P_1 $
                - $ z_2 $ =: Posição, no eixo z, do ponto $ P_2 $
                - $ z_1 $ =: Posição, no eixo z, do ponto $ P_1 $
                - $ w_2 $ =: Posição, no eixo w, do ponto $ P_2 $
                - $ w_1 $ =: Posição, no eixo w, do ponto $ P_1 $
        - Mas, o valor das coordenadas nos eixos x, y e z pertencem aos números reais.
        - Já o valor da cor pode pertencer apenas dentro do intervalo de 0 a 250.
        - Posso dizer que estamos usando dados não normalizados. Que possuem medições percentuais diferentes, dentro dos valores possíveis de cada coordenada.
        - Então, podemos melhorar a fórmula da distância convertendo todos os números das coordenadas para existirem dentro do intervalo de 0 a 1.
        - Normalização de uma coordenada:
            - $ x_{\text{normalizado}} = \frac{x_{medido} - x_{\min}}{x_{\max} - x_{\min}} $
            - Com a normalização, responde-se a pergunta: Qual a porcentagem do valor medido dentro de todos os valores possíveis. A reposta é dada entre 0% e 100%. Perceba que aqui pode-se escolher um valor máximo e um valor mínimo. Ou seja, é necessário conhecer o dado para estas escolhas.
            - Sobre o conhecimento do dado, pode-se também supor que o fato de um dado se localizar dentro de certo intervalo torna o dado mais relevante, mas se apresentar dentro de outra dispersão, o dado passa a não ser tão representativo. Assim, a própria normalização pode ser modificada por um indicar interno de representatividade. Entre valores zero e um, o valor pode aumentar um pouco ou diminuir um pouco, devido esta escolha de representatividade, dentro da dispersão. Mas não mudamos aqui a normalização, e desconsideramos mudanças devido a representatividade.
    - Então, para se ter uma medida de distância entre os dois objetos, cujas coordenada estão normalizadas, calculamos:
        - $ d = \sqrt{({x_2}_{normalizado} - {x_1}_{normalizado})^2 + ({y_2}_{normalizado} - {y_1}_{normalizado})^2 + ({z_2}_{normalizado} - {z_1}_{normalizado})^2 + ({w_2}_{normalizado} - {w_1}_{normalizado})^2 } $
            - Sendo:
                - $ d $ =: distância entre pontos $ P_1 $ e $ P_2 $
                - $ {x_2}_{normalizado} $ =: Posição normalizada, no eixo x, do ponto $ P_2 $
                - $ {x_1}_{normalizado} $ =: Posição normalizada, no eixo x, do ponto $ P_1 $
                - $ {y_2}_{normalizado} $ =: Posição normalizada, no eixo y, do ponto $ P_2 $
                - $ {y_1}_{normalizado} $ =: Posição normalizada, no eixo y, do ponto $ P_1 $
                - $ {z_2}_{normalizado} $ =: Posição normalizada, no eixo z, do ponto $ P_2 $
                - $ {z_1}_{normalizado} $ =: Posição normalizada, no eixo z, do ponto $ P_1 $
                - $ {w_2}_{normalizado} $ =: Posição normalizada, no eixo w, do ponto $ P_2 $
                - $ {w_1}_{normalizado} $ =: Posição normalizada, no eixo w, do ponto $ P_1 $
    - A equação ficou um pouco grande, mas temos uma medida de distância que considera melhor as coordenadas da diferenciação dos corpos.
    - Entretanto, mesmo usando coordenadas normalizadas, pode ser que, na medição, o valor da tonalidade da cor deva ser considerada mais importante do que a medida de distância no eixo y, por exemplo.
    - Ou seja, a medição final da distância depende do valor de importância que damos para cada coordenada.
    - Assim, devemos melhorar ainda mais a fórmula com a ponderação das coordenadas. A distância representará uma comparação entre os corpos, mas considerando o peso percentual que cada coordenada deve ter na caracterização do corpo.
    - Para dar pesos diferentes para as coordenadas, devemos apenas multiplicar todas elas por valores diferentes, que representam sua importância. Por exemplo, podemos multiplicar o x e o y pelo número 2. Mas multiplicamos o Y por 1. E multiplicamos w por 4. Esta escolha reflete uma regra percebida sobre o funcionamento dos dados.
    - Então, para se ter uma medida ponderada da distância entre os dois objetos, cujas coordenadas estão normalizadas, calculamos:
        - $ d = \sqrt{(peso_a . ({x_2}_{normalizado} - {x_1}_{normalizado}))^2 + (peso_b . ({y_2}_{normalizado} - {y_1}_{normalizado}))^2 + (peso_c . ({z_2}_{normalizado} - {z_1}_{normalizado}))^2 + (peso_d . ({w_2}_{normalizado} - {w_1}_{normalizado}))^2 } $
        - Sendo:
            - $ d $ =: distância entre pontos $ P_1 $ e $ P_2 $
            - $ {peso}_a $ =: Peso da medida $ {x}_{normalizado} $ 
            - $ {x_2}_{normalizado} $ =: Posição normalizada, no eixo x, do ponto $ P_2 $
            - $ {x_1}_{normalizado} $ =: Posição normalizada, no eixo x, do ponto $ P_1 $
            - $ {peso}_b $ =: Peso da medida $ {y}_{normalizado} $ 
            - $ {y_2}_{normalizado} $ =: Posição normalizada, no eixo y, do ponto $ P_2 $
            - $ {y_1}_{normalizado} $ =: Posição normalizada, no eixo y, do ponto $ P_1 $
            - $ {peso}_c $ =: Peso da medida $ {z}_{normalizado} $ 
            - $ {z_2}_{normalizado} $ =: Posição normalizada, no eixo z, do ponto $ P_2 $
            - $ {z_1}_{normalizado} $ =: Posição normalizada, no eixo z, do ponto $ P_1 $
            - $ {peso}_d $ =: Peso da medida $ {w}_{normalizado} $ 
            - $ {w_2}_{normalizado} $ =: Posição normalizada, no eixo w, do ponto $ P_2 $
            - $ {w_1}_{normalizado} $ =: Posição normalizada, no eixo w, do ponto $ P_1 $

## Distância entre dois pontos, no espaço de 5D ou de ainda mais coordenadas, com dados normalizados e ponderados
- Segue-se a mesma fórmula do espaço 4D.
- Aplicação desta distância:
    - Pode-se usar esta fórmula para diferenciar diferentes tipos de objetos.
    - Os objetos podem ser matemáticos, físicos, químicos ou mesmo objetos representativos de estruturas sociais. 
    - Os objetos considerados nesta fórmula podem ter 5, 6, ou centenas/milhares de coordenadas diferenciadoras dos objetos.
    - Mas o sistema pode ficar muito complexo se usamos milhares de coordenadas e se tentamos normalizar todas elas e ainda fornecer peso ponderado para cada uma. Entretanto, esta fórmula pode ser muito útil para descrever e caracterizar a aproximação/distância entre objetos.
    - Algoritmos podem ajudar para dar peso e para normalizar os valores das coordenadas.
    - Além disso, sistema de AI podem ser usados para que se descubra, a partir da análise histórica, dentro dos dados estudados, quais as coordenadas relevantes para descrever o sistema, e quais pesos ponderados devem ser usados para diferenciar a importância das coordenadas. Pode-se prever o comportamento de sistemas complexos, a partir desta fórmula. Basta que se debruce sobre os dados e se faça perguntas relevantes e criativas sobre o relacionamento entre os diferentes objetos do espaço estudado.

## Limitações da análise da distância entre dois pontos
- Este cálculo é usado para descrever uma relação entre dois objetos semelhantes. Não é usado para mais de dois objetos. E nem é usado para objetos diferentes. 
- Pode-se analisar diferentes duplas, mas uma dupla por vez, e depois comparando as medições das duplas.
- Pensando na análise social, percebemos que o cálculo da distância pode ser usado para entender partidos políticos, por exemplo. Pode-se tentar descrever a relação entre diferentes partidos políticos e extrapolar a análise para se entender o ambiente político onde estes partidos se encontram. Mas pode ser que a análise deste relacionamento seja insuficiente para a compreensão de todo o sistema político analisado.
- Pode ser que a análise sistêmica requeira a inclusão do objeito "PIB" ou do objeto "Velocidade do Crescimento Econômico", por exemplo. Neste caso, deve-se usar outra ferramenta matemática. O cálculo da distância entre dois pontos executa um cálculo em específico: calcula a relação de aproximação entre dois objetos que possuem os mesmos tipos de coordenadas. 
