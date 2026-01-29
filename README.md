📦 Previsão de Estoque Inteligente com Machine Learning
📌 Visão Geral

Este projeto tem como objetivo desenvolver um Modelo de Machine Learning para Previsão de Estoque Inteligente, aplicando as principais etapas de um pipeline de ML: seleção de dados, treinamento, análise e geração de previsões.

O desafio foi proposto no contexto do Amazon SageMaker Canvas (no-code). No entanto, devido a limitações de acesso à AWS, todo o pipeline foi implementado em Python, replicando de forma fiel e conceitual as etapas do Canvas, garantindo o mesmo aprendizado prático.

🎯 Objetivo do Projeto

Prever a demanda futura de estoque com base em dados históricos

Identificar quais variáveis mais influenciam a previsão

Apoiar a tomada de decisão para reposição de estoque

Consolidar conhecimentos em Machine Learning aplicado

🚀 Passo a Passo do Desenvolvimento
1️⃣ Seleção do Conjunto de Dados

O conjunto de dados utilizado representa um cenário simplificado de controle de estoque, contendo as seguintes variáveis:

data

produto

estoque_atual

vendas_ultimos_30_dias

previsao (variável alvo)

Os dados foram criados e organizados para simular um ambiente real de gestão de estoque, permitindo que o modelo aprendesse padrões de consumo ao longo do tempo.

🔎 Esta etapa equivale à seleção e upload do dataset no SageMaker Canvas.

2️⃣ Construção e Treinamento do Modelo

Nesta etapa, o pipeline de Machine Learning foi desenvolvido utilizando Python e Scikit-learn, contemplando:

Separação entre variáveis de entrada (features) e saída (target)

Codificação de variáveis categóricas

Divisão dos dados em conjuntos de treino e teste

Treinamento do modelo Random Forest Regressor

O algoritmo foi escolhido por sua robustez, bom desempenho em dados tabulares e facilidade de interpretação.

⚙️ Equivalente à etapa Build / Train do SageMaker Canvas.

3️⃣ Análise do Modelo

Após o treinamento, o modelo foi avaliado utilizando a métrica:

MAE (Mean Absolute Error)

Também foi realizada a análise de importância das variáveis, permitindo identificar os fatores mais relevantes para a previsão de estoque.

Principais insights obtidos:

A variável vendas_ultimos_30_dias apresentou maior influência nas previsões

O estoque atual impacta diretamente a necessidade de reposição

O modelo apresentou desempenho satisfatório para o cenário proposto

📊 Equivalente à aba Analyze do SageMaker Canvas.

4️⃣ Previsão de Estoque

Com o modelo treinado e validado, foram realizadas previsões para novos dados de entrada, simulando cenários futuros de demanda.

As previsões permitem:

Antecipar necessidades de reposição

Reduzir riscos de ruptura de estoque

Apoiar decisões estratégicas

🔮 Equivalente à etapa Predict do SageMaker Canvas.

🧠 Conclusões

O modelo desenvolvido demonstrou ser eficaz na previsão de estoque, atendendo aos objetivos propostos no desafio.

Mesmo sem o uso direto da AWS, foi possível:

Reproduzir todas as etapas de um pipeline de ML no-code

Aplicar boas práticas de modelagem

Gerar previsões interpretáveis e úteis para o negócio

Este projeto reforça a aplicabilidade do Machine Learning na área de supply chain e gestão de estoque.

🛠️ Tecnologias Utilizadas

Python

Pandas

Scikit-learn

Google Colab

Machine Learning Supervisionado (Regressão)

▶️ Como Executar o Projeto

Abra o notebook previsao_estoque_ml.ipynb

Execute as células em sequência

📌 Opcional: abrir diretamente no Google Colab

https://colab.research.google.com/github/carioca1965/lab-aws-sagemaker-canvas-estoque/blob/main/previsao_estoque_ml.ipynb

📌 Observações Finais

Caso o acesso ao Amazon SageMaker Canvas estivesse disponível, o mesmo fluxo poderia ser executado integralmente na AWS.
A abordagem adotada garante equivalência técnica e conceitual, mantendo o foco no aprendizado e na entrega do desafio proposto pela DIO.

🤔 Dúvidas?

Em caso de dúvidas ou sugestões:

Abra uma issue neste repositório

Consulte a documentação oficial das bibliotecas utilizadas

🚀 Projeto desenvolvido como parte de um desafio prático da DIO
