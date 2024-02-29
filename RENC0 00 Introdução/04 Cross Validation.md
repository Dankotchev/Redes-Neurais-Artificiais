# *Cross Validation*

***Cross Validation (CV)***  é uma técnica de avaliação de treinamento para aprendizado de máquina que difere do tradicional 70% do *dataset* para treinamento e 30% para testes. No *cross validation* podemos utilizar a técnica de  _k-folds_  onde o *dataset* é dividido em k partes, normalmente entre 5 ou 10 partes, podendo variar conforme o tamanho do conjunto de dados. Cada parte é denominada de fold e possui aproximadamente a mesma quantidade de amostras do conjunto.

![Ilustração do cross validation](https://miro.medium.com/v2/resize:fit:700/1*kkMtezwv8qj1t9uG4nw_8g.png)  

Com os dados divididos em  _folds_, a cada iteração do  **CV**  um  _fold_  é selecionado para ser o conjunto de testes, enquanto os demais k-1  _folds_  são usados para treinamento, gerando assim uma métrica de avaliação. Na iteração seguinte um  _fold_  seguinte é determinado como conjunto de teste e o restante como treinamento.

A saída é um conjunto de métricas relacionadas ao treinamento aplicado, para cada  _fold_  do Cross Validation.

# Referências bibliográficas

LYASHENKO, Vladimir. JHA, Abhishek. **Cross-Validation in Machine Learning: How to Do It Right.** 2023. Disponível em:  [https://neptune.ai/blog/cross-validation-in-machine-learning-how-to-do-it-right](https://neptune.ai/blog/cross-validation-in-machine-learning-how-to-do-it-right). Acesso em: 16 fev. 2024.  

PESSANHA, Cínthia. **Por que cross validation?** 2019. Disponível em:  [https://medium.com/cinthiabpessanha/por-que-cross-validation-b4f57007834a](https://medium.com/cinthiabpessanha/por-que-cross-validation-b4f57007834a). Acesso em: 16 fev. 2024.  

RABELO, Eduardo Braz. **Cross Validation: Avaliando seu modelo de Machine Learning**. 2019. Disponível em:  [https://medium.com/@edubrazrabello/cross-validation-avaliando-seu-modelo-de-machine-learning-1fb70df15b78](https://medium.com/@edubrazrabello/cross-validation-avaliando-seu-modelo-de-machine-learning-1fb70df15b78). Acesso em: 16 fev. 2024.