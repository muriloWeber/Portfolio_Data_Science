# Projeto de Clusterização - Agrupamento de Clientes (Marketing)

## Visão Geral

Este projeto visa analisar dados relacionados aos clientes de cartão de crédito para o Departamento de Marketing, utilizando técnicas de agrupamento para identificar padrões de comportamento e orientar estratégias de marketing.

## Fonte de Dados

Os dados foram obtidos do conjunto disponível no Kaggle, contendo informações sobre o saldo, compras, saques, frequência de compras, entre outros.

Link para os dados no Kaggle (https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)

## Tecnologias Utilizadas

- Linguagem de Programação: Python
- Bibliotecas Principais: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, TensorFlow/Keras
- Ferramentas: Jupyter Notebook, GitHub

## Etapas do Projeto Versão 1 (V1)

1. **Importação e Análise dos Dados**: 
- Os dados foram importados a partir de um arquivo CSV seguido de uma exploração inicial, identificação de valores nulos e tratamento dos mesmos.
- Identificação de clientes com maiores compras à vista e saques de limite.

2. **Visualização dos Dados**: 
- Utilização de gráficos e mapas de calor para visualizar distribuições e identificar padrões.
- Remoção de atributos não relevantes para o algoritmo de agrupamento.

3. **Normalização e Padronização**: 
- Normalização dos dados por padronização para melhor desempenho de algoritmos que calculam distâncias.

4. **Determinação do Número de Clusters**: 
- Utilização do método do cotovelo (Elbow Method) para determinar o número ideal de clusters.

5. **Agrupamento com K-means**: 
- Aplicação do algoritmo K-means para agrupar clientes em clusters.
- Avaliação do modelo utilizando o Silhouette Score.

6. **Análise Preliminar dos Clusters**: 
- Descrição e interpretação dos clusters gerados, identificando padrões de comportamento.

7. **Exportação de Resultados**: 
- Criação de um DataFrame ordenado com os clusters para envio ao Departamento de Marketing.

8. **Aplicação de PCA e Visualização**: Aplicação da técnica PCA para redução de dimensionalidade.
- Visualização dos clusters em um gráfico de dispersão.

9. **Aplicação de Autoencoders**: 
- Utilização de autoencoders para redução de dimensionalidade.
- Escolha do número de clusters com base no Elbow Method aplicado à base compacta.

10. **Exportação Final de Resultados**:
- Criação de um DataFrame ordenado com os clusters gerados pelos autoencoders.


**Conclusões e Recomendações**:
- Este projeto fornece uma visão aprofundada do comportamento dos clientes de cartão de crédito, identificando clusters distintos. As conclusões e recomendações derivadas desses clusters podem ser utilizadas pelo Departamento de Marketing para personalizar estratégias e melhor atender às necessidades dos diferentes perfis de clientes.

**Observações**:
- Este README serve como um guia rápido para entender o projeto. Qualquer dúvida ou necessidade de esclarecimento adicional, favor abrir uma "issue" ou entrar em contato diretamente.

## Limitações e Recomendações (V1)

- O número de clusters foi determinado utilizando o método do cotovelo. No entanto, esse método é apenas uma aproximação e não é garantido que ele irá identificar o número de clusters ideal.

- Essa limitação será abordada na versão 2 do projeto, onde será realizada uma análise mais completa da sensibilidade do modelo ao número de clusters com a inclusão de análise por meio da métrica Silhouette Score.