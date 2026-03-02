# Deal Scoring Preditivo

Inteligência Artificial + Business Intelligence aplicados ao funil de vendas.

<p align="center">
  <img src="visual-dashboard.png" alt="Dashboard Deal Scoring" width="800"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn"/>
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"/>
</p>

## Visão Geral

Este projeto transforma dados de CRM em um **Score de Risco Dinâmico (0-100)** usando Machine Learning, permitindo que equipes comerciais:

- priorizem oportunidades com maior probabilidade de fechamento;
- identifiquem negociações com alto risco de perda;
- tomem decisões orientadas por dados.

A solução conecta modelagem preditiva e visualização estratégica no Power BI.

## Problema de Negócio

Equipes comerciais frequentemente investem tempo em negociações de baixa probabilidade.

Métricas tradicionais são reativas: mostram o que já aconteceu, mas não antecipam resultados.

Perguntas que o projeto responde:

- Qual a probabilidade real de fechamento de um negócio?
- Quais fatores influenciam diretamente o sucesso?

Objetivo: evoluir da análise descritiva para **decisão preditiva acionável**.

## Solução Desenvolvida

A abordagem combina engenharia de dados e Machine Learning para gerar um score confiável, mesmo em cenário desbalanceado.

### Etapas do Modelo

1. Baseline
- Regressão Logística
- Random Forest
- Árvore de Decisão

2. Otimização
- Gradient Boosting (modelo final)
- SMOTE (balanceamento de classes)
- Target Encoding (captura de histórico)

### Resultado Técnico

- +20% de melhoria em ROC-AUC
- Acurácia final: **62,25%**
- Melhor equilíbrio entre classes (Won vs Lost)

## Entrega de Valor (Power BI)

O modelo é operacionalizado em um dashboard interativo com:

- filtros por vendedor, setor e oportunidade;
- identificação visual de risco (baixo, médio, alto);
- priorização de leads em tempo real;
- apoio direto à tomada de decisão.

O modelo deixa de ser apenas técnico e passa a ser uma **ferramenta de gestão**.

## Insights Estratégicos

Principais descobertas:

- **Produto:** `GTX Basic` com maior impacto na conversão (~7,6%);
- **Setores:** tecnologia, software e entretenimento com maior previsibilidade;
- **Vendedores:** padrões individuais influenciam diretamente o sucesso.

> Insight de negócio: direcionar esforços para leads de baixo risco pode aumentar o *win rate* em até **15%**.

## Stack Tecnológica

### Dados e Processamento

- Python
- Pandas
- NumPy

### Machine Learning

- Scikit-learn
- Imbalanced-learn (SMOTE)
- Gradient Boosting

### Visualização

- Power BI
- Seaborn
- Matplotlib

### Pipeline

`ETL -> Feature Engineering -> Modelagem -> Scoring -> Dashboard`

## Estrutura do Projeto

```text
projeto-ml-deal-scoring/
|-- dataset/
|   |-- accounts.csv
|   |-- data_dictionary.csv
|   |-- products.csv
|   |-- sales_pipeline.csv
|   `-- sales_teams.csv
|-- modelo_v1_baseline.ipynb
|-- modelo_v2_otimizado.ipynb
|-- modelo_v3_melhorado.ipynb
|-- pipeline_com_score_v4.csv
|-- negocios_ativos_com_score_risco.csv
|-- deal-scoring.pbix
|-- visual-dashboard.png
`-- README.md
```

## Como Executar

### 1. Clonar o repositório

```bash
git clone https://github.com/karlarenatadev/projeto-ml-deal-scoring.git
cd projeto-ml-deal-scoring
```

### 2. Instalar dependências

```bash
pip install pandas numpy scikit-learn imbalanced-learn seaborn matplotlib
```

### 3. Executar notebooks

Na ordem:

```text
modelo_v1_baseline.ipynb
modelo_v2_otimizado.ipynb
modelo_v3_melhorado.ipynb
```

### 4. Abrir dashboard

Abra `deal-scoring.pbix` no Power BI Desktop.

## Autora

**Karla Renata**

Estudante de Ciência da Computação, focada em transformar dados em decisões estratégicas.
