# Ajuste-de-Hiperpar-metros-e-Avalia-o-de-Modelo-em-Regress-o-Log-stica

O código é um exemplo de classificação binária utilizando o algoritmo de Regressão Logística, uma técnica de Machine Learning. O conjunto de dados utilizado é gerado aleatoriamente para fins de demonstração. O conjunto de dados consiste em 1000 exemplos, cada um com quatro características e uma classe de destino.

O código começa dividindo os dados em conjuntos de treinamento e teste com uma divisão de 80/20 usando a função train_test_split do sklearn. Ele utiliza um pipeline do sklearn para realizar a padronização dos dados (pré-processamento) e aplicar o modelo de Regressão Logística.

Para ajustar os hiperparâmetros do modelo, o código utiliza a técnica de busca em grade (GridSearchCV) sobre um conjunto predefinido de hiperparâmetros. A busca em grade treina o modelo para cada combinação de parâmetros e seleciona a que oferece o melhor desempenho, com base na validação cruzada.

A acurácia do modelo é avaliada comparando as previsões do modelo (obtidas aplicando o modelo aos dados de teste) com os valores reais (rótulos de classe dos dados de teste). A acurácia é a proporção de previsões corretas entre todas as previsões realizadas.

Além da acurácia, o código calcula a matriz de confusão e a exibe como um heatmap. A matriz de confusão é uma tabela que descreve o desempenho de um modelo de classificação, mostrando o número de verdadeiros positivos, verdadeiros negativos, falsos positivos e falsos negativos.

O código também gera uma Curva ROC (Receiver Operating Characteristic). A curva ROC é um gráfico que mostra o desempenho de um modelo de classificação em todos os limiares de classificação. A AUC (Área Sob a Curva) é uma métrica de desempenho que resume a curva ROC: uma AUC de 1.0 indica um modelo perfeito, enquanto uma AUC de 0.5 indica um modelo aleatório.

Finalmente, o modelo treinado é salvo em um arquivo usando a biblioteca pickle, para que possa ser reutilizado posteriormente sem a necessidade de treinamento adicional.
