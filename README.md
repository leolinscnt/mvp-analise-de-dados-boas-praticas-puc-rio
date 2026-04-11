# Análise de Dados - Resultados de Jogos da NBA

Aluno: Leonardo Cantisano Lins

Matrícula: 4052025001952

Dataset: NBA Games Data

## Objetivo

Este projeto tem como objetivo deste trabalho é analisar os dados históricos de jogos para identificar padrões e relações entre variáveis estatísticas e o resultado das partidas, com foco especial na influência do desempenho do time mandante em relação ao visitante.


## Definição do Problema

O problema consiste em identificar quais métricas estatísticas estão mais associadas às vitórias dos times mandantes, considerando dados históricos de partidas da NBA.

Trata-se de um problema de **classificação supervisionada**, com variável alvo binária indicando vitória (1) ou derrota (0) do time mandante.


## Principais Hipóteses

- Times mandantes possuem maior probabilidade de vitória;
- Times mandantes tendem a apresentar pontuação média superior;
- A probabilidade de vitória está mais associada à eficiência de arremessos (FG%) do que a métricas isoladas de pontuação;
- O desempenho relativo entre as equipes (diferença entre métricas de mandante e visitante) é mais relevante para explicar o resultado do que métricas isoladas;
- Times com maior volume de assistências tendem a apresentar melhor desempenho e maior probabilidade de vitória;
- A capacidade das arenas tem influência no resultado das partidas.


## Análise Exploratória

Durante a análise, foram identificados os seguintes insights:

- Existe vantagem estatística para o time mandante;
- A eficiência de arremessos (FG%) possui a maior correlação com o resultado;
- O número de assistências possui forte correlação com o número de pontos;
- A eficiência de arremessos (FG%) de um time e o número de rebotes obtidos pelo adversário apresentam relevante correlação negativa;
- A diferença entre métricas de desempenho (mandante vs visitante) é o principal fator explicativo;
- Rebotes possuem impacto secundário no resultado da partida, apresentando maior dispersão;
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
