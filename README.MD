# AI Jobs Market Analysis (2025-2026)

**Dataset:** [IA Jobs Market 2025 and 2026](https://www.kaggle.com/datasets/alitaqishah/ai-jobs-market-2025-2026-salaries)

**Colab MVP:** https://colab.research.google.com/github/LucasDSF7/Data-Analysis-Puc-Rio/blob/master/ia_jobs_market.ipynb

## MVP: Análise de Dados e Boas Práticas — PUC-Rio

Este projeto apresenta uma análise exploratória e o pré-processamento de um dataset contendo 1.500 anúncios de emprego nas áreas de Inteligência Artificial e Machine Learning. O foco principal é entender os fatores que influenciam a remuneração e validar hipóteses sobre o mercado de trabalho global.

## Descrição do Problema

O objetivo central é a previsão salarial baseada em características como função, país, nível de experiência e competências. O conjunto de dados abrange:

    Período: 2025 - 2026.

    Escopo: 25 funções em 14 países.

    Variáveis: Salários, competências (skills), tendências de trabalho remoto, porte da empresa...

## Hipóteses e Resultados

Durante a análise, cinco hipóteses principais foram testadas:

    Tendência de cargos de LLM: Não foi identificada uma tendência de crescimento proporcional clara ao longo do tempo para vagas específicas de LLM.

    Anos vs. nível de experiência: O número de anos de experiência exigido não possui correspondência direta com o nível de senioridade (Entry, Mid, Senior, Lead).

    Habilidade mais requisitada: Python confirmou-se como a habilidade mais requisitada no mercado de IA/ML.

    Distorções salariais: Existem diversas situações em que um anúncio Entry level supera o salário de anúncios Senior/Lead.

    Tendência geográfica para vagas de LLM: Foi possível mapear e identificar países com maior concentração de vagas voltadas para Large Language Models.

## Pré-processamento e Insights

A análise revelou que variáveis categóricas como company_size e country são preditores mais fortes para o salário anual do que as variáveis numéricas isoladas.

Principais técnicas aplicadas:

    Ordinal Encoding: Aplicado a atributos categóricos ordinais para preservar a hierarquia de pesos.

    Feature Transformation: Tratamento da coluna required_skills para extração de dados significativos.

    Escalonamento: Aplicação de técnicas de escalonamento para alimentar modelos de ML.

## Trabalhos Futuros

    Implementar Feature Engineering com dados temporais.

    Refinar a transformação de required_skills para mitigar riscos de Data Leakage.

    Testar diferentes algoritmos de normalização para otimizar a performance do modelo preditivo.

    Implementar diferentes modelos de ML para prever o salário de vagas de IA/ML.

## Estrutura do Repositório

📁 DATA-ANALYSIS-PUC-RIO/
│-- 📂 data_exploratory_analysis_and_pre_processing/  # Pasta com exercícios das aulas da disciplina EDA e Pre Processing
│-- 📂 data_visualization/                            # Pasta com exercícios das aulas da disciplina Data Visualization
│-- 📂 mvp/                                           # Pasta com notebooks e bases de dados do MVP
│-- 📄 ia_jobs_market.ipynb                           # Link Google Colab do notebook do MVP
│-- 📄 README.md                                      # Documentação do projeto
│-- 📄 requiriments.txt                               # Dependências do projeto

## Instalação de Dependências

    Criar ambiente virtual com Python 3.11
    bash: pip install -r requirements.txt