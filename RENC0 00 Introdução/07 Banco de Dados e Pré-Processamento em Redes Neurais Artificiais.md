
# Banco de dados e pré-processamento em redes neurais artificiais

## Banco de dados

Um banco de dados é essencial para o treinamento eficaz de uma rede neural artificial (RNA) devido à sua capacidade de fornecer uma variedade de dados de treinamento que representam a realidade a qual será submetida a RNA em ambiente de produção. Além disso, um banco de dados robusto contribui para o desenvolvimento de modelos de RNA mais precisos e confiáveis, uma vez que a qualidade e a quantidade dos dados são fundamentais para o sucesso do treinamento.

Quanto mais diversos forem os exemplos encontrados no banco de dados, menos viés poderá ser desenvolvido durante a fase de treinamento, quanto mais vasto um conjunto de dados for menor é a chance de ocorrer overfitting em cima dos dados, o que levará a uma rede neural artificial, mas ajustada, permitindo que ocorram menos erros durante o teste e uso do modelo treinado.

## Pré-processamento

Durante a etapa de treinamento a rede neural artificial (RNA) recebe inúmeros padrões de dados, com diversas características, entretanto muitas dessas informações carregam pouca informação para formação do treinamento, comumente caracterizado como informações de baixa entropia (Moutinho; Neto, 2002), que eventualmente podem confundir a rede neural artificial.

Um método utilizado para reduzir a dimensão dos dados é conhecido por “redução de dimensões por componentes principais (ou análise de componentes principais – PCA) que objetiva “transformar um conjunto de dados de alta dimensionalidade em um novo conjunto de dimensão ortogonal, chamadas de ‘componente principal’” (Almeida, 2023).

Outra técnica de pré-processamento capaz de reduzir o tamanho das entradas, principalmente imagens, é a decomposição e compressão de Wavelet, ou Transformada de Wavelet. A aplicação da transformada Wavelet em imagens digitais permite compressão sem perda de informação (Universidade Fernando Pessoa, 2024) que ao ser aplicada nas entradas reduz a dimensão das amostras pela metade (sendo na verdade duas saídas: uma que contém a amostra geral do sinal e outra detalhada) e podendo reconstruir a imagem original (Moutinho; Neto, 2002).

No trabalho de Moutinho e Neto (2002) ambos métodos foram utilizados para investigar se há vantagens em pré-processar um conjunto de imagens de dígitos de 0 a 9, que passaram por uma rede neural de 64 neurônios de entrada, duas camadas intermediárias de 20 neurônios cada e 10 neurônios na saída, representando cada um dos dígitos. A conclusão obtida foi que aplicar qualquer um dos métodos isoladamente obteve menos erros de reconhecimento na fase de teste da rede, e a combinação de transformada de Wavelet e PCA obteve 83% de resultados corretos, o melhor desempenho observado (Moutinho; Neto, 2002) a tabela abaixo compila os resultados encontrados pelos autores.

![Resultados comparativo entre métodos de pré-processamento](https://images2.imgbox.com/59/39/Mu9pv2p1_o.png)

## Referências

ALMEIDA, Vitor. Redução de dimensionalidade no aprendizado de máquina. _In_: Blog Gran Cursos Online. 31 ago. 2023. Disponível em: https://blog.grancursosonline.com.br/reducao-de-dimensionalidade-no-aprendizado-de-maquina/. Acesso em: 8 mar. 2024.

MOUTINHO, Adriano; NETO, Luiz. Métodos de Pré-Processamento de Sinais Aplicados ao Treinamento de Redes Neurais Artificiais. _In_: II CONGRESSO BRASILEIRO DE COMPUTAÇÃO, 2002. **Anais [...]**. 2002. Disponível em: https://www.researchgate.net/publication/228521586_METODOS_DE_PRE-PROCESSAMENTO_DE_SINAIS_APLICADOS_AO_TREINAMENTO_DE_REDES_NEURAIS_ARTIFICIAIS. Acesso em: 8 mar. 2024.

UNIVERSIDADE FERNANDO PESSOA. **Transformadas Wavelet**. 2024. Disponível em: http://multimedia.ufp.pt/codecs/compressao-com-perdas/transformadas-wavelet/. Acesso em: 8 mar. 2024.