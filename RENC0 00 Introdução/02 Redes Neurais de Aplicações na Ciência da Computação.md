# Redes neurais aplicadas na computação

O trabalho de Ferneda (2006) é um exemplo de redes neurais artificiais utilizada para a recuperação de informações, que em termos práticos trata-se de buscar documentos que atendam a determinados "termos de busca". A RNA consiste em três camada, uma entrada de com os termos de busca, uma camada de saída com os documentos e na camada central os termos de indexação, a figura 1 representa tal rede.

![Representação de rede neural aplicada à recuperação de informação](https://images2.imgbox.com/99/53/pssZe6rM_o.png)  

O processo inicia a partir dos termos de busca, ativando neurônios intermediários dos conjuntos de termos de indexação, que enviam para sinais para os documentos. A rede retorna sinais de ativação dos documentos para os termos de indexação a fim de refinar as saídas.

A cada interação os sinais de ativação dos documentos para os termos indexadores ficam mais fracos, e em algum momento são cessados, desta forma a rede termina de operar, e tem como saídas documentos que refletem os termos buscados, sejam de forma direta ou indireta, a partir de inferências que a própria rede criou.

Outras aplicações de RNA é apresentada no trabalho de Aderaldo (2017) onde cita diversas aplicações de redes neurais para a detecção de intrusão e anomalias em redes de computadores. Entre os métodos apresentados são utilizadas redes neurais de múltiplas camadas, redes neurais de Kohonen, árvores de decisão e perceptron.

# Referências bibliográficas

ADERALDO, V. P.  **Utilização de Redes Neurais Artificiais para Detecção de Anomalia** **em Redes de computadores**. 58p. Trabalho de Conclusão de Curso (Bacharelado em Ciência da Computação) – Universidade Estadual de Londrina, Londrina-PR, 2017. Disponível em: [https://www.uel.br/cce/dc/wp-content/uploads/VersaoPreliminarTCC-VITOR_PALMA_ADERALDO.pdf](https://www.uel.br/cce/dc/wp-content/uploads/VersaoPreliminarTCC-VITOR_PALMA_ADERALDO.pdf). Acesso em: 9 fev. 2024.  

FERNEDA, E.  **Redes neurais e sua aplicação em sistemas de recuperação de informação**. Ciência da Informação, [S. l.], v. 35, n. 1, 2006. DOI: 10.18225/ci.inf.v35i1.1149. Disponível em: [https://revista.ibict.br/ciinf/article/view/1149](https://revista.ibict.br/ciinf/article/view/1149). Acesso em: 9 fev. 2024.