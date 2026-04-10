# Análise de Dados - Resultados de Jogos da NBA

Aluno: Leonardo Cantisano Lins

Matrícula: 4052025001952

Dataset: NBA Games Data

## Objetivo

Este projeto tem como objetivo analisar os fatores que influenciam o resultado de partidas de basquete da NBA (liga de basquete dos Estados Unidos), com foco na comparação entre o desempenho de times mandantes e visitantes.


## Definição do Problema

O problema consiste em identificar quais métricas estatísticas estão mais associadas às vitórias dos times mandantes, considerando dados históricos de partidas da NBA.

Trata-se de um problema de **classificação supervisionada**, com variável alvo binária indicando vitória (1) ou derrota (0) do time mandante.


## Principais Hipóteses

- Times mandantes possuem maior probabilidade de vitória;
- O desempenho relativo entre as equipes é mais relevante do que métricas isoladas;
- Métricas de eficiência ofensiva possuem maior impacto no resultado;
- A capacidade das arenas não influencia significativamente o resultado.


## Análise Exploratória

Durante a análise, foram identificados os seguintes insights:

- Existe vantagem estatística para o time mandante;
- A eficiência de arremessos (FG%) possui forte relação com o resultado;
- A diferença entre métricas de desempenho (mandante vs visitante) é o principal fator explicativo;
- Rebotes possuem impacto secundário;
- Capacidade das arenas não apresentou relevância significativa.


## Pré-processamento

Foram realizadas as seguintes etapas:

- Tratamento de valores nulos;
- Criação de variáveis derivadas (diferenças entre equipes);
- Separação entre treino e teste;
- Padronização das variáveis numéricas (StandardScaler).


## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn


## Como Executar

1. Abra o notebook no Google Colab;
2. Execute as células sequencialmente;
3. Os dados são carregados diretamente via URL do GitHub.


## Estrutura do Projeto

- Notebook com todas as etapas:
  - Definição do problema
  - Análise exploratória
  - Pré-processamento
  - Conclusão


## Conclusão

O estudo demonstrou que o desempenho relativo entre as equipes é o principal fator associado ao resultado das partidas, sendo mais relevante do que métricas isoladas.

Além disso, foi possível validar quantitativamente hipóteses que, embora intuitivas, ganham robustez quando analisadas sob a ótica de dados.
