# Olá, eu sou Josafha Pereira de Carvalho 👋

**Estudante de Engenharia da Computação | Ciência de Dados & Machine Learning**

🎓 Graduando no 7º semestre de Engenharia da Computação pela Universidade Federal do Pará (UFPA). Tenho interesse em Ciência de Dados, Machine Learning e Engenharia de Dados, com projetos que passam por análise exploratória, preparação dos dados, modelagem, validação e integração de modelos em aplicações.

🔬 Fui bolsista de Iniciação Científica (PIBIC) no laboratório MensureLab (UFPA), atuando no desenvolvimento de códigos para tratamento de dados, mineração de texto e Reconhecimento de Entidades Nomeadas (NER). Também atuei no desenvolvimento de dashboards e participei da escrita de um artigo científico.

---

## 🛠️ Stack Tecnológico

| Área | Tecnologias |
| --- | --- |
| **Linguagens** | Python, SQL (SQLite) |
| **Machine Learning** | XGBoost, Random Forest, Scikit-Learn, SVM, Prophet |
| **Análise e Processamento de Dados** | Pandas, NumPy, SciPy, Expressões Regulares |
| **Visualização de Dados** | Tableau, Matplotlib, Seaborn |
| **Infraestrutura e Ferramentas** | Git, GitHub, Linux, venv, Docker, Docker Compose, RabbitMQ, MongoDB, Jupyter, VS Code e Google Colab |

## 📊 Métodos e Avaliação

| Área | Experiência prática |
| --- | --- |
| **Classificação** | F1 Macro, matriz de confusão, validação por blocos temporais |
| **Regressão** | R², MAE, RMSE, validação cruzada K-Fold, Feature Importance, Permutation Importance |
| **Séries Temporais** | Validação cruzada temporal, MAE, MAPE, RMSE, cobertura do intervalo de incerteza |
| **Estatística** | Regressão Linear, correlação de Pearson e Spearman, Informação Mútua, Agrupamento Hierárquico, ANOVA, ANOVA de Welch, teste de Levene e teste de Shapiro-Wilk |
| **Processamento de Sinais** | Filtros Butterworth, FFT, janelamento deslizante, autocorrelação e entropia espectral |
| **Análise Exploratória** | Boxplots, scatter plots, histogramas, mapas de correlação, gráficos de séries temporais e análise gráfica de resíduos |

---

## 🚀 Principais Projetos

### 📦 N.O.V.A — Inteligência Artificial aplicada à Gestão de Estoque

[**Ver projeto no GitHub**](https://github.com/Josafha-pereira/stockly-ia)

Projeto desenvolvido no contexto da Stockly, um sistema acadêmico de gestão de estoque para supermercados. A N.O.V.A reúne dois serviços de Machine Learning voltados à classificação das condições de armazenamento de frutas e à previsão de demanda.

Na classificação, desenvolvi quatro modelos XGBoost especializados por fruta, utilizando temperatura, umidade e CO₂ como variáveis de entrada. O processo incluiu análise exploratória, preparação dos dados, treinamento, validação e exportação dos modelos finais.

Na previsão de demanda, utilizei Prophet com modelos separados por loja e produto. A pesquisa incluiu análise das séries temporais, validação cruzada temporal, avaliação com MAE, MAPE, RMSE e cobertura do intervalo de incerteza, além da geração de previsões futuras.

Também implementei dois microserviços para execução dos modelos, com solicitações recebidas pelo RabbitMQ e resultados armazenados no MongoDB. Os serviços foram containerizados com Docker e Docker Compose, formando um ambiente local que simula o fluxo de produção.

**Principais tecnologias**

`Python` `XGBoost` `Prophet` `Pandas` `Scikit-Learn` `RabbitMQ` `MongoDB` `Docker` `Docker Compose`

---

### ⚖️ Predição de Criminalidade Violenta em Comunidades dos EUA

[**Ver projeto no GitHub**](https://github.com/Josafha-pereira/Modelagem-Preditiva-de-Criminalidade)

Projeto de Machine Learning para estimar a taxa de criminalidade violenta de comunidades a partir de características socioeconômicas, demográficas e de estrutura familiar.

A análise exploratória envolveu prevenção de data leakage, filtro de completude, seleção de variáveis com Informação Mútua e agrupamento hierárquico para redução de redundância. A variável categórica `State` foi avaliada com teste de Levene e ANOVA de Welch, resultando em nove preditores selecionados a partir das 147 variáveis originais.

Na modelagem, comparei XGBoost Regressor e Random Forest Regressor por desempenho e estabilidade em validação cruzada K-Fold. Também foram analisados overfitting, regularização de hiperparâmetros, Feature Importance e Permutation Importance.

O XGBoost apresentou R² médio de 0,66 e desvio padrão de 0,033 entre os folds. O modelo final foi treinado com as 1.395 comunidades disponíveis para treino e validação e utilizado para gerar previsões para outras 599 comunidades mantidas fora da análise e do treinamento.

**Principais tecnologias**

`Python` `XGBoost` `Random Forest` `Scikit-Learn` `Pandas` `NumPy` `SciPy` `Matplotlib` `Seaborn`

---

### 🏃‍♂️ Reconhecimento de Atividades Humanas (HAR)

[**Ver projeto no GitHub**](https://github.com/Josafha-pereira/Reconhecimento-de-Atividades-Humanas-HAR)

Projeto de Processamento Digital de Sinais e Machine Learning para classificação de três atividades humanas — caminhada, corrida e salto — a partir de dados coletados por um acelerômetro triaxial.

O processamento inclui filtros Butterworth passa-alta e passa-baixa, janelamento deslizante com 75% de overlap e extração de 15 características estatísticas e espectrais, incluindo média, desvio padrão, autocorrelação, pico FFT e entropia espectral.

Foram comparados SVM, Random Forest e XGBoost utilizando F1 Macro e validação em cinco folds formados por blocos temporais. Para evitar compartilhamento de amostras entre treino e validação, janelas de treino sobrepostas aos blocos de validação são removidas em cada fold.

O Random Forest apresentou o maior F1 Macro médio, com 0,77, seguido pelo XGBoost, com 0,73, e pelo SVM, com 0,68. A variação entre os folds foi alta nos três modelos, principalmente devido à quantidade reduzida de janelas disponíveis para avaliação.

**Principais tecnologias**

`Python` `NumPy` `Pandas` `SciPy` `Scikit-Learn` `XGBoost` `SVM` `Random Forest` `Matplotlib` `Seaborn`
