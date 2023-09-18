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

## Etapas do Projeto Versão 1 (V1)

1. **Importação e Análise dos Dados**: Os dados foram importados a partir de um arquivo CSV e uma análise inicial foi realizada para entender a estrutura da base de dados.

2. **Visualização dos Dados**: Foram criadas visualizações e gráficos para explorar os dados e identificar padrões relevantes.

3. **Pré-processamento dos Dados**: Os dados foram pré-processados para prepará-los para o treinamento do modelo. Isso incluiu a conversão de variáveis categóricas em variáveis dummy e a normalização das variáveis numéricas.

4. **Modelagem e Avaliação**: Foram treinados diferentes modelos de machine learning, incluindo Regressão Logística, Random Forest e Redes Neurais Artificiais. Métricas de desempenho, como acurácia, precisão, recall e pontuação F1, foram calculadas para avaliar os modelos.

5. **Salvando o Modelo**: O modelo de Regressão Logística foi escolhido como o modelo final devido ao seu melhor desempenho. O modelo treinado e os objetos de pré-processamento foram salvos em um arquivo para uso futuro.

6. **Simulação de Execução do Modelo**: Uma simulação foi demonstrada usando um novo registro da base de dados para mostrar como o modelo pode ser utilizado para fazer previsões.

## Base de Dados Desbalanceada

É importante observar que a base de dados utilizada neste projeto está desbalanceada, ou seja, há um desequilíbrio significativo entre as classes de funcionários que saíram da empresa (classe positiva) e os que ficaram (classe negativa). Esse desbalanceamento pode afetar o desempenho do modelo de machine learning, levando a resultados enviesados.

## Versão 2 (V2) - Aplicação de Oversampling para Balanceamento da classe a ser prevista**

Os três primeiros itens da versão 1 foram mantidas na versão 2, abaixo segue as principais mudanças na V2:

**Oversampling para Balanceamento de Dados:**
Nesta versão do projeto, foi aplicada a técnica de oversampling para balancear a classe minoritária em relação à classe majoritária. Isso ajuda a melhorar o desempenho do modelo em dados desbalanceados.

**Random Forest:**
Um modelo de Random Forest foi treinado, utilizando os dados de treinamento, e avaliado, utilizando os dados de teste. Métricas de desempenho, como precisão, recall, F1 Score e acurácia, foram calculadas para avaliar o modelo. O Random Forest demonstrou um desempenho excepcional na identificação de funcionários propensos a deixar a empresa.

**Random Forest com Bootstrap Bagging (Tentativa de Redução de Variabilidade):**
No modelo de Random Forest, foi realizada uma tentativa de reduzir a variabilidade na validação cruzada por meio da técnica de Bootstrap Bagging. No entanto, essa tentativa não teve sucesso.

**Rede Neural Artificial (MLP):**
Uma rede neural artificial (MLP) foi implementada e treinada com diferentes camadas e neurônios. O modelo MLP alcançou um equilíbrio entre precisão e recall, tornando-o eficaz na identificação de funcionários propensos a sair.

**Análise de Overfitting:**
Foram realizadas análises de overfitting para avaliar a capacidade de generalização dos modelos. No geral, os modelos não apresentaram sinais significativos de overfitting.

**Busca de Melhor Combinação de Hiperparâmetros:**
Para o modelo de Random Forest, uma busca de hiperparâmetros foi realizada para encontrar a melhor combinação de parâmetros e melhorar o desempenho.

**Escolha do Melhor Modelo:**
A rede neural artificial (MLP) foi escolhida como o modelo final devido ao seu melhor desempenho geral e equilíbrio entre precisão e recall.

**Conclusão:**
Este projeto evoluiu com a aplicação de técnicas avançadas, resultando em um modelo de previsão mais preciso e eficaz para o Departamento de Recursos Humanos. A escolha do modelo final levou em consideração o equilíbrio entre precisão e recall, garantindo que os funcionários propensos a deixar a empresa sejam identificados com alta precisão.
