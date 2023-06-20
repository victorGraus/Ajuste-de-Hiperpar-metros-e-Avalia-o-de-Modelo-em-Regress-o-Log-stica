# Ajuste-de-Hiperpar-metros-e-Avalia-o-de-Modelo-em-Regress-o-Log-stica
Text português BR e Inglês

The code is an example of binary classification using the Logistic Regression algorithm, a Machine Learning technique. The dataset used is randomly generated for demonstration purposes. The dataset consists of 1000 examples, each with four features and a target class.

The code begins by splitting the data into training and test sets with an 80/20 split using the train_test_split function from sklearn. It uses an sklearn pipeline to perform data standardization (preprocessing) and apply the Logistic Regression model.

To tune the model's hyperparameters, the code uses the grid search technique (GridSearchCV) over a predefined set of hyperparameters. The grid search trains the model for each parameter combination and selects the one that offers the best performance based on cross-validation.

The model's accuracy is evaluated by comparing the model's predictions (obtained by applying the model to the test data) with the actual values (class labels of the test data). Accuracy is the proportion of correct predictions out of all predictions made.

In addition to accuracy, the code calculates the confusion matrix and displays it as a heatmap. The confusion matrix is a table that describes the performance of a classification model, showing the number of true positives, true negatives, false positives, and false negatives.

The code also generates a Receiver Operating Characteristic (ROC) curve. The ROC curve is a graph that shows the performance of a classification model at all classification thresholds. The Area Under the Curve (AUC) is a performance metric that summarizes the ROC curve: an AUC of 1.0 indicates a perfect model, while an AUC of 0.5 indicates a random model.

Finally, the trained model is saved to a file using the pickle library so that it can be reused later without the need for additional training.


PTBR
O código é um exemplo de classificação binária utilizando o algoritmo de Regressão Logística, uma técnica de Machine Learning. O conjunto de dados utilizado é gerado aleatoriamente para fins de demonstração. O conjunto de dados consiste em 1000 exemplos, cada um com quatro características e uma classe de destino.

O código começa dividindo os dados em conjuntos de treinamento e teste com uma divisão de 80/20 usando a função train_test_split do sklearn. Ele utiliza um pipeline do sklearn para realizar a padronização dos dados (pré-processamento) e aplicar o modelo de Regressão Logística.

Para ajustar os hiperparâmetros do modelo, o código utiliza a técnica de busca em grade (GridSearchCV) sobre um conjunto predefinido de hiperparâmetros. A busca em grade treina o modelo para cada combinação de parâmetros e seleciona a que oferece o melhor desempenho, com base na validação cruzada.

A acurácia do modelo é avaliada comparando as previsões do modelo (obtidas aplicando o modelo aos dados de teste) com os valores reais (rótulos de classe dos dados de teste). A acurácia é a proporção de previsões corretas entre todas as previsões realizadas.

Além da acurácia, o código calcula a matriz de confusão e a exibe como um heatmap. A matriz de confusão é uma tabela que descreve o desempenho de um modelo de classificação, mostrando o número de verdadeiros positivos, verdadeiros negativos, falsos positivos e falsos negativos.

O código também gera uma Curva ROC (Receiver Operating Characteristic). A curva ROC é um gráfico que mostra o desempenho de um modelo de classificação em todos os limiares de classificação. A AUC (Área Sob a Curva) é uma métrica de desempenho que resume a curva ROC: uma AUC de 1.0 indica um modelo perfeito, enquanto uma AUC de 0.5 indica um modelo aleatório.

Finalmente, o modelo treinado é salvo em um arquivo usando a biblioteca pickle, para que possa ser reutilizado posteriormente sem a necessidade de treinamento adicional.
