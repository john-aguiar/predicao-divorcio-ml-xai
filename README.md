# Predictive factors of divorce: an approach using machine learning and explainable artificial intelligence

Este repositório contém a tabela de descrição dos 54 atributos do conjunto de dados, gráficos, binário dos modelos de Machine Learning e script Colab.

O artigo, fruto de Trabalho de Conclusão de Curso do curso de Bacharelado em Ciência da Computação, foi submetido a <a href="https://seer.ufrgs.br/index.php/rita/about"> <strong>Revista de Informática Teórica e Aplicada (RITA)</strong></a>

Os autores do artigo foram:

* **João Victor Albuquerque de Aguiar** (autor principal) contribuiu para a redação do manuscrito, executou os experimentos computacionais e participou da revisão do artigo.
* **Adonias Caetano de Oliveira** revisou o manuscrito e os experimentos computacionais, atuando como orientador e coordenador do projeto de pesquisa.
* **Rhyan Ximenes de Brito**, **Paulo Ricardo Barboza Gomes** e **Benedito Gomes Rodrigues** revisaram o manuscrito e os resultados obtidos.

 ## 📋 Requisitos de bibliotecas Python

* import gdown
* import os
* import pickle
* import pandas as pd
* import numpy as np
* import xgboost as xgb
* import random
* from sklearn.model_selection import train_test_split
* from sklearn.metrics import accuracy_score
* from sklearn.metrics import classification_report, confusion_matrix, ConfusionMatrixDisplay
* from sklearn.model_selection import GridSearchCV
* import shap
* import seaborn as sns
* import matplotlib.pyplot as plt
* from lime.lime_tabular import LimeTabularExplainer
* from sklearn.svm import SVC
* from xgboost import XGBClassifier
* from sklearn.naive_bayes import GaussianNB
* from sklearn.neural_network import MLPClassifier
* from sklearn.ensemble import RandomForestClassifier
* from sklearn.linear_model import LogisticRegression
* from IPython.display import display

## 📖  Conjunto de Dados

O conjunto de dados <a href="https://archive.ics.uci.edu/dataset/539/divorce+predictors+data+set"><strong>Divorce Predictors dataset</strong></a>,  disponibilizado publicamente pelo UCI Machine Learning Repository, foi composto por 170 registros de casais, com 54 atributos. Dos participantes, 49% eram divorciados e 51% eram casados, sendo 86 homens e 84 mulheres, com idades variando de 20 a 63 anos. Os registros contêm respostas na escala ordinal na faixa de 0 a 4, correspondentes às opções do questionário que utilizava a escala Likert. 

## 🛠 Ajuste fino dos modelos

Nós avaliamos os algoritmos de Machine Learning Random Forest (RF), Support Vector Machine (SVM), Multilayer Perceptron (MLP), Naive Bayes  (NB) e eXtreme Gradient Boosting (XGBoost). As experimentações utilizaram uma combinação de 10-Fold Cross-Validation e Hold-Out para garantir confiabilidade no treinamento e robustez na avaliação final. O conjunto de dados foi inicialmente dividido de forma estratificada em treino e teste, considerando três proporções: 80/20, 50/50 e 20/80. Durante o treinamento, os dados de treino foram novamente particionados em 80% para treinamento e 20% para validação, aplicando K-Fold (k=10). A otimização dos hiperparâmetros foi realizada por meio de Grid Search. Após o ajuste fino, os modelos foram avaliados no conjunto de teste correspondente ao hold-out inicial.

## 🤖 Artigo em processo de revisão da RITA

### [Paper Link]() 

## Contribuições

Se houver um bug ou outra melhoria que você gostaria de relatar ou solicitar, nós o encorajamos a contribuir.

Por favor, sinta-se à vontade para entrar em contato conosco para quaisquer perguntas: [![Gmail Badge](https://img.shields.io/badge/-adonias.oliveira@ifce.edu.br-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:adonias.oliveira@ifce.edu.br)](mailto:adonias.oliveira@ifce.edu.br )

[Clique aqui para acessar o dataset traduzido em formato PDF](tabela_DPS.pdf)

