# Projeto de Previsão de Evasão de Clientes

## Descrição do Projeto

Este é um projeto de Machine Learning que visa construir modelos preditivos para prever quais clientes de uma empresa de telecomunicações têm maior probabilidade de cancelar seus serviços (evadir). A antecipação da evasão permite que a empresa implemente estratégias de retenção proativas e direcionadas, visando diminuir a perda de clientes.

O projeto envolve as seguintes etapas principais:

- Exploração e Preparação de Dados: Carregamento, limpeza, transformação e codificação do conjunto de dados de clientes.
- Análise de Dados: Investigação das relações entre variáveis e identificação de fatores que influenciam a evasão.
- Modelagem Preditiva: Desenvolvimento e treinamento de modelos de Machine Learning para prever a evasão.
- Avaliação do Modelo: Análise do desempenho dos modelos utilizando métricas relevantes.
- Interpretação e Recomendações: Compreensão dos resultados dos modelos e proposição de estratégias de retenção.

## Modelos de Machine Learning Utilizados

Neste projeto, utilizamos os seguintes modelos de classificação para prever a evasão de clientes:

- Regressão Logística: Um modelo linear que estima a probabilidade de um cliente evadir com base nas características de entrada. É útil por sua interpretabilidade, pois os coeficientes indicam a direção e a força da relação entre as variáveis e a probabilidade de evasão.
- Random Forest: Um modelo de conjunto que constrói múltiplas árvores de decisão. Ele combina as previsões de árvores individuais para melhorar a robustez e a precisão. É eficaz para capturar relações não-lineares nos dados e fornece uma medida de importância das variáveis.

## Avaliação do Desempenho dos Modelos

Para avaliar o quão bem nossos modelos preveem a evasão, utilizamos métricas comuns em problemas de classificação:

- Acurácia (Accuracy): A proporção de previsões corretas (clientes que evadiram e foram previstos como evasão, e clientes que não evadiram e foram previstos como não-evasão) em relação ao total de previsões. Embora seja uma métrica geral, em conjuntos de dados desbalanceados (onde uma classe é muito mais frequente que a outra), a acurácia pode ser enganosa.
- Precisão (Precision): Das previsões de evasão feitas pelo modelo, quantos realmente evadiram. É uma medida de quão confiáveis são as previsões positivas (evasão) do modelo. Alta precisão significa menos falsos positivos (prever evasão quando o cliente não evadiu).
- Recall (Sensibilidade): Dos clientes que realmente evadiram, quantos o modelo conseguiu identificar corretamente. É uma medida da capacidade do modelo de encontrar todos os casos positivos (evasão). Alto recall significa menos falsos negativos (não prever evasão quando o cliente evadiu).
- F1-score: A média harmônica da Precisão e do Recall. É uma métrica que busca um equilíbrio entre Precisão e Recall, sendo útil especialmente em conjuntos de dados desbalanceados.
- Matriz de Confusão (Confusion Matrix): Uma tabela que resume o desempenho de um modelo de classificação. Ela mostra o número de verdadeiros positivos (TP), verdadeiros negativos (TN), falsos positivos (FP) e falsos negativos (FN).
    - Verdadeiro Positivo (TP): O modelo previu evasão, e o cliente realmente evadiu.
    - Verdadeiro Negativo (TN): O modelo previu não-evasão, e o cliente realmente não evadiu.
    - Falso Positivo (FP): O modelo previu evasão, mas o cliente não evadiu (Erro Tipo I).
    - Falso Negativo (FN): O modelo previu não-evasão, mas o cliente evadiu (Erro Tipo II).

## Definições de Machine Learning

- Machine Learning (Aprendizado de Máquina): Um campo da inteligência artificial que permite que sistemas aprendam com dados, identifiquem padrões e tomem decisões com o mínimo de intervenção humana.
- Modelo Preditivo: Um modelo matemático ou computacional treinado em dados históricos para fazer previsões sobre eventos futuros ou resultados desconhecidos.
- Classificação: Um tipo de problema de Machine Learning onde o objetivo é prever a qual categoria discreta um ponto de dado pertence (neste caso, "Evasão" ou "Não Evasão").
- Overfitting: Ocorre quando um modelo aprende demais os detalhes e o ruído dos dados de treinamento, resultando em um desempenho ruim em dados novos e não vistos.
- Underfitting: Ocorre quando um modelo é muito simples para capturar as complexidades e padrões dos dados de treinamento, resultando em um desempenho ruim tanto nos dados de treino quanto nos dados de teste.
