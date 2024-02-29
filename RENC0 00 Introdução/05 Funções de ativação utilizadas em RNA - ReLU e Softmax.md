# Funções de ativação utilizadas em RNA: ReLU e Softmax

## Introdução

As funções de ativação são ferramentas matemáticas que introduzem não-linearidade nas saídas de cada camada de uma rede neural artificial, desempenhando um papel permitindo que neurônios decidam se devem ser ativados ou não com base nas informações recebidas. Possibilitando que pequenas alterações nos pesos e  _bias_  resultem em mudanças proporcionais nas saídas, facilitando o processo de aprendizagem.

As funções lineares, embora constante em seu gradiente, ou seja, produzindo saídas proporcionais as entradas,  é  útil para tarefas simples, mas inadequada para redes mais profundas. Por outro lado, as funções sigmoides, amplamente utilizada, proporciona suavidade e não-linearidade, embora possa enfrentar problemas com gradientes pequenos e mapeando valores para um intervalo especifico, como entre 0 e 1, -1 e 1, sendo úteis para problemas de classificação, para além de desempenhar um papel essencial na capacidade das redes neurais de resolver problemas complexos, como tradução de idiomas e classificação de imagens.

## Função ReLU

A função  _rectified linear unit,_ ou unidade linear retificada conhecida por ReLU produz resultados dentro do intervalo entre 0 e infinito positivo, através da fórmula  **g(u) = max (0, u)**, ou seja, retornando valor zero para quaisquer valores negativos. Sendo atualmente a função de ativação mais utilizada.

![Função ReLU](https://miro.medium.com/v2/resize:fit:720/format:webp/0*17a9Xr_jp1KXlxT8.png)  

Como produz valores zeros para resultados negativos, no processo de  _feedforward_ alguns neurônios tendem a não ser ativados, ocasionando em uma rede mais esparsa e eficiente para computação. Entretanto essa não ativação de um neurônio pode ser considerada uma desvantagem, podendo os pesos deste neurônio não serem atualizados, deixando “mortos”.

Para resolver esse problema causado por saídas zeros, foi proposta a  **Leaky ReLU**  que define um pequeno componente para valores negativos, resultando na fórmula  **g(u) = max (au, u)**, para u < 0 e  **g(u) = max (0, u)**  para u > 0, onde  _a_  pode ser entendido como um valor próximo de zero, e, portanto, todos os valores resultantes da função de ativação, quando diferentes de 0, resultaram em ativações de neurônios a frente.

![Função Leaky ReLU](https://miro.medium.com/v2/resize:fit:4800/format:webp/0*H0IL4cgGNp9vEwJh.png)  

## Função Softmax

A função Softmax é aplicada em redes neurais artificiais para classificação e é entendida como uma generalização da função sigmoide para casos não binários, costumadamente aplicadas a camada de saída de uma rede neural, permitindo lidar com múltiplas classes. A saída da função (valores entre 0 e 1, que somados resultam em 1) pode ser entendida como a probabilidade das entradas de pertencerem a uma determinada classe.

![Função Softmax](https://www.deeplearningbook.com.br/wp-content/uploads/2018/02/softmax.png)  

# Referências bibliográficas

CECCON, Denny.  **Funções de ativação: definição, características, e quando usar cada uma**. [_S. l._], 2020. Disponível em:  [https://iaexpert.academy/2020/05/25/funcoes-de-ativacao-definicao-caracteristicas-e-quando-usar-cada-uma/](https://iaexpert.academy/2020/05/25/funcoes-de-ativacao-definicao-caracteristicas-e-quando-usar-cada-uma/). Acesso em: 16 fev. 2024.

DATA SCIENCE ACADEMY. Capítulo 8 - Função de Ativação.  _In_: DEEP LEARNING BOOK. [_S. l._]: Data Science Academy, 2022. Disponível em:  [https://www.deeplearningbook.com.br/funcao-de-ativacao/](https://www.deeplearningbook.com.br/funcao-de-ativacao/). Acesso em: 16 fev. 2024.

ESTEVES, Toni.  **A desvantagem da função ReLU.**  [_S. l._], 2022. Disponível em:  [https://estevestoni.medium.com/a-desvantagem-de-utilizar-relu-4478589ef834](https://estevestoni.medium.com/a-desvantagem-de-utilizar-relu-4478589ef834). Acesso em: 16 fev. 2024.

FACURE, Matheus.  **Funções de Ativação**. [_S. l._], 2017. Disponível em:  [https://matheusfacure.github.io/2017/07/12/activ-func/](https://matheusfacure.github.io/2017/07/12/activ-func/). Acesso em: 16 fev. 2024.

GOODFELLOW, Ian; BENGIO, Yoshua; COURVILLE, Aaron.  **Deep Learning**. [_S. l._]: MIT Press, 2016. Disponível em:  [https://www.deeplearningbook.org](https://www.deeplearningbook.org/). Acesso em: 17 fev. 2024.