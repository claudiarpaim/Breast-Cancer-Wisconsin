# Diagnóstico de Câncer de Mama com Machine Learning

<p align="center">
  <img src="cover_breast_cancer_ml.png" width="500">
</p>

# Visão Geral

Este projeto tem como objetivo desenvolver e avaliar modelos de Machine Learning supervisionado para classificar tumores mamários como benignos ou malignos, utilizando dados extraídos de exames citológicos. O estudo utiliza o dataset Breast Cancer Wisconsin (Diagnostic), amplamente empregado em pesquisas acadêmicas e aplicações educacionais em ciência de dados.

O projeto segue uma abordagem estruturada baseada na metodologia CRISP-DM, cobrindo desde a compreensão do problema até a avaliação dos modelos.

# Problema de Negócio

O diagnóstico precoce e preciso do câncer de mama é fundamental para aumentar as chances de tratamento eficaz e reduzir a mortalidade. Métodos automatizados baseados em Machine Learning podem auxiliar profissionais da saúde ao oferecer suporte à decisão, reduzindo erros humanos e agilizando análises diagnósticas.

# Dataset

- Fonte: Breast Cancer Wisconsin (Diagnostic)

- Origem: Kaggle / UCI Machine Learning Repository

- Amostras: 569

- Variável alvo: Malignant (M)/ Benign (B)

- Características: 30 atributos numéricos derivados de imagens de núcleos celulares (raio, textura, perímetro, área, suavidade, concavidade, entre outros).

# Metodologia

O projeto foi desenvolvido seguindo as etapas abaixo:

### 1 - Entendimento dos dados

- Análise da estrutura do dataset

- Verificação de tipos, valores ausentes e distribuição das classes

### 2 - Análise Exploratória de Dados (EDA)

- Estatísticas descritivas

- Visualização da distribuição das variáveis

- Análise de correlação entre atributos

### 3 - Pré-processamento

- Separação em conjuntos de treino e teste

- Escalonamento das variáveis

- Avaliação de possíveis impactos de outliers

### 4 - Modelagem

- Regressão Logística

- Support Vector Machine (SVM)

- Random Forest

- XGBoost

### 5 - Avaliação

- Acurácia

- Precisão

- Recall

- F1-score

- Matriz de confusão

- Validação cruzada

- Ajuste de hiperparâmetros

# Resultados

Os modelos apresentaram alto desempenho na classificação, com destaque para algoritmos baseados em ensemble e métodos de margem máxima, que obtiveram melhor equilíbrio entre precisão e recall, métricas críticas em problemas de diagnóstico médico.

Os resultados indicam que técnicas de Machine Learning podem ser ferramentas eficazes no apoio à identificação precoce do câncer de mama.

# Tecnologias Utilizadas

- Python

- NumPy

- Pandas

- Matplotlib

- Seaborn

- Scikit-learn

- XGBoost
