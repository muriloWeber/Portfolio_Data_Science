# Projeto de Previsão de Classificação - Atrito de Funcionários

## Visão Geral

Este é um projeto de previsão de classificação desenvolvido para ajudar o Departamento de Recursos Humanos a identificar funcionários propensos a deixar a empresa. O projeto utiliza técnicas de aprendizado de máquina e é direcionado ao Departamento de Recursos Humanos (RH) de uma organização.

## Fonte de Dados

- [IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- [Cálculo de Salário](https://www.mom.gov.sg/employment-practices/salary/monthly-and-daily-salary) e [How to Calculate for the Daily Rate from Your Monthly Salary](https://sprout.zendesk.com/hc/en-us/articles/360030922133-How-to-Calculate-for-the-Daily-Rate-from-Your-Monthly-Salary-)
- [Stock Options](https://www.moneyunder30.com/employee-stock-options#:~:text=Typically%20they%20are%20granted%20to,a%20specific%20period%20of%20time.)

## Tecnologias Utilizadas

- Linguagem de Programação: Python
- Bibliotecas Principais: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, TensorFlow/Keras
- Ferramentas: Jupyter Notebook, GitHub

## Etapas do Projeto

1. **Importação e Análise dos Dados**: Os dados foram importados a partir de um arquivo CSV e uma análise inicial foi realizada para entender a estrutura da base de dados.

2. **Visualização dos Dados**: Foram criadas visualizações e gráficos para explorar os dados e identificar padrões relevantes.

3. **Pré-processamento dos Dados**: Os dados foram pré-processados para prepará-los para o treinamento do modelo. Isso incluiu a conversão de variáveis categóricas em variáveis dummy e a normalização das variáveis numéricas.

4. **Modelagem e Avaliação**: Foram treinados diferentes modelos de machine learning, incluindo Regressão Logística, Random Forest e Redes Neurais Artificiais. Métricas de desempenho, como acurácia, precisão, recall e pontuação F1, foram calculadas para avaliar os modelos.

5. **Salvando o Modelo**: O modelo de Regressão Logística foi escolhido como o modelo final devido ao seu melhor desempenho. O modelo treinado e os objetos de pré-processamento foram salvos em um arquivo para uso futuro.

6. **Simulação de Execução do Modelo**: Uma simulação foi demonstrada usando um novo registro da base de dados para mostrar como o modelo pode ser utilizado para fazer previsões.

## Base de Dados Desbalanceada

É importante observar que a base de dados utilizada neste projeto está desbalanceada, ou seja, há um desequilíbrio significativo entre as classes de funcionários que saíram da empresa (classe positiva) e os que ficaram (classe negativa). Esse desbalanceamento pode afetar o desempenho do modelo de machine learning, levando a resultados enviesados.

## Possível Versão Futura (V2)

Uma possível melhoria para este projeto seria abordar o problema do desbalanceamento da base de dados. Isso pode ser feito por meio de técnicas de balanceamento de dados, como oversampling da classe minoritária, undersampling da classe majoritária ou o uso de algoritmos de aprendizado de máquina projetados para lidar com dados desbalanceados.

Futuras versões deste projeto podem explorar essas técnicas e avaliar seu impacto no desempenho do modelo, buscando obter previsões mais precisas e úteis para o RH da empresa. Esta é uma área de aprimoramento importante para tornar o projeto ainda mais eficaz.
