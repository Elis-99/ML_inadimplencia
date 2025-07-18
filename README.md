Previsão de Inadimplência para Locadora de Automóveis
Este projeto utiliza machine learning para prever inadimplência de clientes de uma locadora de veículos.

Metodologia
Balanceamento: NearMiss (v3)

Classificador: DecisionTreeClassifier (max_depth=10)

Avaliação: matriz de confusão, métricas de classificação (acurácia, precisão, recall, F1-score, AUC, AP)

Resultados
Acurácia de validação: 0.91

Acurácia em teste: 0.91

Precisão: 0.25

Recall: 0.04

F1-Score: 0.07

AUC: 0.52

AP: 0.09

Matriz de Confusão
Previsto 0	Previsto 1
Real 0	10355	124
Real 1	960	42
Métricas detalhadas (max_depth=10)
Classe	Precisão	Recall	F1-score	Suporte
0	0.94	0.48	0.64	7397
1	0.12	0.70	0.20	707
Acurácia geral			0.50	8104
Média macro F1-score: 0.42

Média ponderada F1-score: 0.60

Uso
Clone este repositório ou baixe o .ipynb.

Instale dependências:

pip install scikit-learn imbalanced-learn pandas matplotlib
Execute o notebook.


Observações
O modelo apresenta bom desempenho em identificar a classe majoritária, mas performance baixa na minoria (inadimplentes).
