# Análise de Dados - Resultados de Jogos da NBA

**Aluno:** Leonardo Cantisano Lins  
**Matrícula:** 4052025001952  


## Sumário

- [Objetivo](#objetivo)
- [Definição do Problema](#definição-do-problema)
- [Fonte dos Dados](#fonte-dos-dados)
- [Acesso ao Notebook](#acesso-ao-notebook)
- [Principais Hipóteses](#principais-hipóteses)
- [Análise Exploratória](#análise-exploratória)
- [Pré-processamento](#pré-processamento)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Executar](#como-executar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Conclusão](#conclusão)


## Objetivo

Este projeto tem como objetivo analisar os dados históricos de jogos para identificar padrões e relações entre variáveis estatísticas e o resultado das partidas, com foco especial na influência do desempenho do time mandante em relação ao visitante.


## Definição do Problema

O problema consiste em identificar quais métricas estatísticas estão mais associadas às vitórias dos times mandantes, considerando dados históricos de partidas da NBA.

Trata-se de um problema de **classificação supervisionada**, com variável alvo binária indicando vitória (1) ou derrota (0) do time mandante.


## Fonte dos Dados

Os dados utilizados neste projeto foram obtidos a partir do seguinte dataset no Kaggle:

https://www.kaggle.com/datasets/nathanlauga/nba-games

Os arquivos foram posteriormente disponibilizados via GitHub para garantir a reprodutibilidade da análise.


## Acesso ao Notebook

Notebook no GitHub:  
https://github.com/leolinscnt/mvp-analise-de-dados-boas-praticas-puc-rio/blob/main/notebooks/mvp_analise_de_dados.ipynb  

Abrir diretamente no Google Colab:  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/leolinscnt/mvp-analise-de-dados-boas-praticas-puc-rio/blob/main/notebooks/mvp_analise_de_dados.ipynb)


## Principais Hipóteses

- Times mandantes possuem maior probabilidade de vitória;
- Times mandantes tendem a apresentar pontuação média superior;
- A probabilidade de vitória está mais associada à eficiência de arremessos (FG%) do que à pontuação absoluta;
- O desempenho relativo entre as equipes (diferença entre métricas de mandante e visitante) é mais relevante para explicar o resultado do que métricas isoladas;
- Times com maior volume de assistências tendem a apresentar melhor desempenho e maior probabilidade de vitória;
- A capacidade das arenas exerce influência sobre o resultado das partidas.


## Análise Exploratória

Durante a análise, foram identificados os seguintes insights:

- Existe vantagem estatística para o time mandante;
- A eficiência de arremessos (FG%) possui forte relação com o resultado;
- A eficiência de arremessos de um time e os rebotes do adversário apresentam correlação negativa;
- Métricas de desempenho relativo (mandante vs visitante) são os principais fatores explicativos;
- Assistências refletem a qualidade do jogo coletivo e estão associadas a melhores resultados;
- Rebotes possuem impacto secundário, com maior dispersão;
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

Além disso, a análise evidenciou a interdependência entre métricas do jogo, como a relação entre eficiência de arremessos e rebotes, e o papel das assistências na qualidade ofensiva das equipes.

Por fim, foi possível validar quantitativamente hipóteses que, embora intuitivas, ganham maior robustez quando analisadas sob a ótica de dados.
