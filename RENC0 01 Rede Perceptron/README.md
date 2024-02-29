# Implementação Computacional da Rede Neural Artificial Perceptron

A indústria Gelatina Ltda. está analisando a possibilidade de implementação de uma rede neural Perceptron para controlar (ligar ou desligar) o motor de um processo específico de sua linha de produção. Durante o período de 1 mês realizou-se a aquisição dos dados relativos às variáveis de entrada (Pressão e Temperatura) e saída (Acionamento do motor), ou seja, monitorou-se o comportamento do processo. Neste sentido, implemente computacionalmente uma rede Perceptron para que sejam realizadas as etapas de treinamento e teste. As/os amostras/padrões representativas/os do comportamento do sistema estão dispostas/os no arquivo em anexo. Ademais, considere as informações abaixo:

 - Valores iniciais dos pesos e bias: definir pseudo-aleatoriamente entre 0 e 1;
 - **Taxa de aprendizagem**: definida pelo usuário (para definir a taxa de aprendizagem reflita sobre a questão da estabilidade da rede neural artificial);
 - Percentual de amostras para os subconjuntos de treinamento e de teste: definido pelo usuário, com base no proposto em literaturas especializadas;
 - **Função de ativação:** degrau;
 - Apresentar ao usuário o tempo de processamento da etapa de treinamento;
 - Apresentar ao usuário o tempo de processamento do teste, considerando a análise de apenas 1 amostra/padrão;
 - Apresentar ao usuário o número de épocas que foram necessárias para realizar o treinamento;
 - Apresentar ao usuário o percentual de acerto obtido na etapa de teste (considerando todo o subconjunto de teste);
 - Apresentar a matriz de confusão.
 
 Por fim, deve-se **plotar 2 gráficos** conforme especificado abaixo:
 - **1º gráfico:** plotar os dados do subconjunto de treinamento (ex: dados relativos às saídas iguais a 0 devem ser plotados como “X” e dados relativos às saídas iguais a 1 devem ser plotados como “.”) e também a reta advinda dos parâmetros da rede Perceptron (reta obtida por meio do valor final dos pesos e bias (valores estes obtidos na última iteração do processo de treinamento));
 - **2º gráfico:** plotar os dados do subconjunto de teste (ex: dados relativos às saídas 0 devem ser plotados como “X” e dados relativos às saídas 1 devem ser plotados como “.”) e também a reta advinda dos parâmetros da rede Perceptron (reta obtida por meio do valor final dos pesos e bias (valores estes obtidos na última iteração do processo de treinamento)).

*Obs 1:* O uso do “X” e “.” é apenas uma sugestão, podem ser utilizados outros indicativos desde que o indicativo das saídas iguais a 0 seja distinto do indicativo das saídas iguais a 1, como por exemplo, plotar os pontos relativos às saídas 0 em ‘vermelho’ e os referentes às saídas iguais a 1 em ‘azul’.

*Obs 2:* Após a conclusão do programa, realize diversas simulações com diferentes valores da taxa de aprendizagem/treinamento e analise o efeito da mesma.