## Pipeline Analítico de Risco de Crédito

Este projeto implementa um **pipeline completo de crédito** para análise de risco de empréstimos, desde a leitura dos dados até a geração de métricas e arquivos prontos para dashboard (Power BI).

---

## Base de Dados

Os dados utilizados neste projeto foram obtidos do **Kaggle**:  
[LoanStats3a - Kaggle](https://www.kaggle.com/datasets/irisk9/loanstats3a)

---

## Funcionalidades

- Upload de arquivo CSV (`LoanStats.csv`) e verificação automática.  
- Pré-processamento de dados (tratamento de nulos, seleção de features).  
- Treinamento e avaliação de modelos de Machine Learning:  
  - Logistic Regression  
  - XGBoost  
- Cálculo de métricas de performance:  
  - AUC, Gini, KS, PR-AUC  
  - Precision, Recall, F1-score, Accuracy  
  - Lift e captura do top decil  
- Geração de arquivos prontos para visualização em Power BI:  
  - `loan_scored.csv` → dados com score do modelo  
  - `model_metrics.csv` → métricas de performance  
  - `data_quality_summary.csv` → resumo da qualidade dos dados  
  - `dashboard_table.csv` → tabela consolidada para dashboards  

---

## Tecnologias Utilizadas

- Python 3.10+  
- [pandas](https://pandas.pydata.org/)  
- [numpy](https://numpy.org/)  
- [scikit-learn](https://scikit-learn.org/stable/)  
- [xgboost](https://xgboost.readthedocs.io/)  
- [matplotlib](https://matplotlib.org/) / [seaborn](https://seaborn.pydata.org/) (opcional para gráficos)  
- Power BI (para visualização e dashboards)  

---

## Como usar

1. Faça upload do arquivo `LoanStats.csv`.
2. Execute o notebook para gerar:  
   - Arquivo scored com predições  
   - Métricas do modelo  
   - Resumo de qualidade dos dados  
   - Tabela final para dashboard  

3. Importe os arquivos gerados no Power BI para criar visualizações.

---

## Executar no Google Colab

Clique no botão abaixo para abrir o notebook no Google Colab:

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/eduardaqueiroga/pipeline-analitico-risco-credito/blob/main/pipeline_analitico_risco_credito.ipynb) 
