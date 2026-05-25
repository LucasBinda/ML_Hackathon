# ML_Hackathon
 Análise Exploratória e Modelagem Preditiva: Mercado Imobiliário

Este projeto foi desenvolvido como parte das avaliações de Ciência de Dados, com o objetivo de explorar, tratar e aplicar algoritmos de Machine Learning sobre um conjunto de dados do mercado imobiliário. O pipeline abrange desde a análise estatística inicial até o uso de técnicas avançadas de aprendizado supervisionado e não supervisionado.
 Estrutura do Projeto e Etapas

O desenvolvimento do notebook foi dividido em 5 etapas fundamentais:

    1. Análise Exploratória de Dados (EDA): Identificação de distribuições, assimetrias e presença de outliers multivariados através de resumos estatísticos e visualizações gráficas (como histogramas e mapas de calor de valores faltantes).

    2. Engenharia de Features: Tratamento personalizado de dados nulos (imputação por contexto de bairro), codificação manual de variáveis ordinais de qualidade, criação de novas métricas imobiliárias (ex: Idade do Imóvel, Área Útil Total) e normalização de escala (StandardScaler).

    3. Aprendizado Supervisionado (Regressão e Classificação):

        Regressão: Modelagem preditiva do preço de venda (SalePrice) utilizando Regressão Linear e Random Forest Regressor.

        Classificação: Transformação do problema para categorizar imóveis de "Alto" ou "Baixo" padrão, comparando Regressão Logística, KNN e Random Forest Classifier através de matrizes de confusão.

    4. Aprendizado Não Supervisionado: Segmentação de mercado sem rótulos prévios utilizando K-Means (3 clusters), redução de dimensionalidade com PCA para visualização espacial, descoberta de padrões com Apriori (Regras de Associação) e detecção de anomalias com LOF (Local Outlier Factor).

    5. Avaliação e Conclusões: Análise comparativa dos modelos utilizando métricas robustas (R2, RMSE, MAE, Acurácia e F1-Score).

 Principais Resultados

    Fatores Determinantes: A qualidade geral do acabamento (OverallQual) e o tamanho da área viva (TotalSF) são os maiores influenciadores no valor dos imóveis.

    Alta Performance: Os modelos de regressão superaram a marca de 0.80 de R2, enquanto o classificador Random Forest atingiu um F1-Score superior a 0.90 na identificação do padrão dos imóveis.

    Consistência Visual: O PCA confirmou que a divisão de mercado em 3 faixas de preço proposta pelo K-Means possui forte separação matemática.

 Tecnologias Utilizadas

    Linguagem: Python

    Manipulação e Visualização: Pandas, NumPy, Matplotlib, Seaborn

    Machine Learning: Scikit-Learn

    Mineração de Dados: Mlxtend

    Como rodar o projeto

    Instale as dependências: pip install pandas numpy matplotlib seaborn scikit-learn mlxtend

    Abra o Jupyter Notebook e execute as células sequencialmente para acompanhar o Storytelling dos dados.
