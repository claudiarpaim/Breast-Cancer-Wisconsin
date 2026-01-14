# Projeto Breast Cancer Wisconsin (Diagnostic)

<p align="center">
  <img src="images/ultrassonografia_mama_ia.png" alt="Capa do projeto" width="800"/>
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

- Os atributos apresentados nos conjunto de dados são:

| Atributo                  | Descrição                                         |
|----------------------------|--------------------------------------------------|
| id                         | Identificador único da amostra                  |
| diagnosis                  | Diagnóstico do tumor: M = Maligno, B = Benigno  |
| radius_mean                | Média da distância do centro aos pontos da borda do núcleo |
| texture_mean               | Média do desvio padrão dos valores de escala de cinza |
| perimeter_mean             | Média do perímetro do núcleo                     |
| area_mean                  | Média da área do núcleo                          |
| smoothness_mean            | Média da variação local do comprimento do raio  |
| compactness_mean           | Média de (perímetro² / área − 1)                |
| concavity_mean             | Média da gravidade das porções côncavas do contorno |
| concave points_mean        | Média do número de pontos côncavos              |
| symmetry_mean              | Média da simetria do núcleo                      |
| fractal_dimension_mean     | Média da dimensão fractal do contorno           |
| radius_se                  | Erro padrão do raio                              |
| texture_se                 | Erro padrão da textura                           |
| perimeter_se               | Erro padrão do perímetro                         |
| area_se                     | Erro padrão da área                              |
| smoothness_se              | Erro padrão da suavidade                         |
| compactness_se             | Erro padrão da compactação                        |
| concavity_se               | Erro padrão da concavidade                        |
| concave points_se          | Erro padrão dos pontos côncavos                  |
| symmetry_se                | Erro padrão da simetria                           |
| fractal_dimension_se       | Erro padrão da dimensão fractal                  |
| radius_worst               | Maior valor do raio observado                    |
| texture_worst              | Maior valor da textura                            |
| perimeter_worst            | Maior valor do perímetro                          |
| area_worst                 | Maior valor da área                               |
| smoothness_worst           | Maior valor da suavidade                          |
| compactness_worst          | Maior valor da compactação                         |
| concavity_worst            | Maior valor da concavidade                         |
| concave points_worst       | Maior número de pontos côncavos                  |
| symmetry_worst             | Maior valor da simetria                           |
| fractal_dimension_worst    | Maior valor da dimensão fractal                  |


# Metodologia

O projeto foi desenvolvido seguindo as etapas abaixo:

### 1 - Entendimento dos dados

- Análise da estrutura do dataset

- Verificação de tipos, valores ausentes e distribuição das classes

### 2 - Análise Exploratória de Dados (EDA)

- Estatísticas descritivas

- Visualização da distribuição das variáveis

<p align="center">
  <img src="images/outliers.png" alt="Capa do projeto" width="700"/>
</p>

- Análise de correlação entre atributos

### 3 - Pré-processamento

- Separação em conjuntos de treino e teste

- Escalonamento das variáveis

- Avaliação de possíveis impactos de outliers

### 4 - Modelagem

- Regressão Logística

- Support Vector Machine (SVM)

<p align="center">
  <img src="images/permutation_importance_svm.png" alt="Capa do projeto" width="600"/>
</p>

- Random Forest

- XGBoost

### 5 - Avaliação

- Acurácia

- Precisão

- Recall

- F1-score

- Matriz de confusão

<p align="center">
  <img src="images/confusion_matrix.png" alt="Capa do projeto" width="400"/>
</p>

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
