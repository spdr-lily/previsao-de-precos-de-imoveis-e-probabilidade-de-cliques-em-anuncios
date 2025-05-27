## **Projeto de Previsão de Preços de Imóveis e Probabilidade de Cliques em Anúncios**

### **1\. Introdução**

Este projeto, é a realização de uma atividade prática, onde se aplicam técnicas de regressão linear e logística em dados simulados. O objetivo é prever o preço de imóveis com base em suas características e a probabilidade de cliques em anúncios, utilizando regressão linear para a previsão de preços e regressão logística para a probabilidade de cliques. O projeto utiliza dados fictícios para demonstrar a aplicação das técnicas de modelagem preditiva.

### **2\. Contexto**

A análise preditiva é essencial para empresas em diversos setores.

* **Parte 1:** No setor imobiliário, a capacidade de prever preços de imóveis com base em suas características permite uma avaliação mais precisa e eficiente dos ativos, auxiliando compradores, vendedores e corretores.  
* **Parte 2:** No marketing digital, prever a probabilidade de cliques em anúncios ajuda a otimizar campanhas, direcionar recursos para os anúncios mais eficazes e melhorar o retorno sobre o investimento.

### **3\. Conjunto de Dados**

O projeto utiliza conjuntos de dados fictícios gerados para simular cenários reais.

* **Parte 1 (Regressão Linear):**  
  * `Numero_Quartos`: Número de quartos do imóvel.  
  * `Metragem_Quadrada`: Metragem quadrada do imóvel.  
  * `Preco_Imovel`: Preço do imóvel.  
* **Parte 2 (Regressão Logística):**  
  * `Idade`: Idade do usuário.  
  * `Renda`: Renda do usuário.  
  * `Clicou`: Variável binária indicando se o usuário clicou no anúncio (1) ou não (0).

### **4\. Metodologia**

O projeto foi desenvolvido em Python e utilizando as bibliotecas pandas, numpy, matplotlib, seaborn e scikit-learn. A metodologia foi dividida em duas partes:

* **Parte 1 (Regressão Linear):**  
  1. Geração de dados fictícios para as variáveis `Numero_Quartos`, `Metragem_Quadrada` e `Preco_Imovel`.  
  2. Divisão dos dados em conjuntos de treinamento e teste.  
  3. Treinamento de um modelo de regressão linear para prever `Preco_Imovel`.  
  4. Avaliação do modelo utilizando o Erro Médio Quadrático (MSE) e o Coeficiente de Determinação (R²).  
  5. Visualização dos dados e do modelo de regressão.  
* **Parte 2 (Regressão Logística):**  
  1. Geração de dados fictícios para as variáveis `Idade`, `Renda` e `Clicou`.  
  2. Análise exploratória dos dados utilizando estatísticas descritivas e visualizações.  
  3. Divisão dos dados em conjuntos de treinamento e teste.  
  4. Treinamento de um modelo de regressão logística para prever a probabilidade de cliques.  
  5. Avaliação do modelo utilizando acurácia, relatório de classificação e matriz de confusão.

### **5\. Implementação**

A implementação do projeto envolveu as seguintes etapas e funções:

* **5.1 Importação das Bibliotecas:**  
  * Foram importadas as bibliotecas pandas para manipulação de dados, numpy para operações numéricas, matplotlib.pyplot e seaborn para visualização, e scikit-learn para modelagem e avaliação.  
* **5.2 Geração de Dados Fictícios:**  
  * A função `numpy.random.randint()` foi utilizada para gerar dados aleatórios para as variáveis independentes.  
  * A variável dependente `Preco_Imovel` foi calculada com base em uma fórmula linear com adição de ruído aleatório.  
  * A função `numpy.random.choice()` foi usada para gerar dados binários aleatórios para a variável `Clicou`.  
* **5.3 Divisão dos Dados:**  
  * A função `train_test_split()` do `scikit-learn` foi utilizada para dividir os dados em conjuntos de treinamento e teste, garantindo que o modelo seja avaliado em dados não vistos durante o treinamento.  
* **5.4 Treinamento do Modelo:**  
  * Para a regressão linear, a classe `LinearRegression()` do `scikit-learn` foi utilizada para criar e treinar o modelo.  
  * Para a regressão logística, a classe `LogisticRegression()` do `scikit-learn` foi utilizada.  
* **5.5 Avaliação do Modelo:**  
  * Para a regressão linear, as funções `mean_squared_error()` e `r2_score()` do `scikit-learn.metrics` foram utilizadas para calcular o Erro Médio Quadrático (MSE) e o Coeficiente de Determinação (R²), respectivamente.  
  * Para a regressão logística, as funções `accuracy_score()`, `classification_report()` e `confusion_matrix()` do `scikit-learn.metrics` foram utilizadas para avaliar o desempenho do modelo.  
* **5.6 Visualização dos Dados:**  
  * Foram criados gráficos de dispersão para visualizar a relação entre as variáveis na regressão linear.  
  * Foi utilizado `seaborn.pairplot()` para visualizar a distribuição e relação entre as variáveis na regressão logística.  
  * Foi gerado um mapa de calor da matriz de confusão para visualizar o desempenho do modelo de regressão logística.

### **6\. Resultados**

Os resultados obtidos com a análise incluem:

* **Parte 1 (Regressão Linear):**  
  * Erro Médio Quadrático (MSE): Quantifica o erro médio das previsões do modelo.  
  * Coeficiente de Determinação (R²): Mede a proporção da variância na variável dependente que é previsível a partir das variáveis independentes.  
* **Parte 2 (Regressão Logística):**  
  * Acurácia: Proporção de previsões corretas do modelo.  
  * Relatório de Classificação: Métricas como precisão, recall e F1-score para cada classe.  
  * Matriz de Confusão: Visualização do número de previsões corretas e incorretas.

### **7\. Conclusão**

Este projeto demonstrou a aplicação de técnicas de regressão linear e logística para prever preços de imóveis e a probabilidade de cliques em anúncios, utilizando dados fictícios. As funções implementadas permitiram a geração, manipulação, modelagem, avaliação e visualização dos dados, fornecendo insights sobre as relações entre as variáveis e o desempenho dos modelos preditivos.
