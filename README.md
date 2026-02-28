# 🚀 Deal Scoring Preditivo: Inteligência Artificial no Funil de Vendas

Este projeto utiliza **Machine Learning** para transformar dados estáticos de um CRM num **Score de Risco Dinâmico (0-100)**. A solução permite que equipas comerciais priorizem oportunidades com maior probabilidade de fecho e identifiquem antecipadamente negócios em risco de perda.

---

## 📌 Contexto e Problema de Negócio
No cenário comercial tradicional, métricas como "Dias na Etapa" servem apenas como alertas passivos. O desafio deste projeto foi criar um modelo preditivo capaz de analisar o comportamento histórico de vendas e responder:
* **Qual é a probabilidade real deste negócio ser ganho?**
* **Quais fatores (produto, setor, vendedor) mais influenciam o sucesso?**

A inovação aqui reside em converter dados descritivos em **estatística acionável**, integrando o resultado diretamente num dashboard de Business Intelligence.

---

## 🛠️ Stack Tecnológica
* **Linguagem:** Python 3.14.0
* **Bibliotecas de ML:** Scikit-learn, Pandas, Numpy.
* **Algoritmos Testados:** Regressão Logística, Random Forest, Decision Tree e Gradient Boosting.
* **Visualização de Dados:** Power BI, Seaborn, Matplotlib.
* **Workflow:** ETL -> Feature Engineering -> Model Selection -> Exportação para BI.

---

## 📊 Performance e Batalha de Modelos
Para garantir a melhor precisão no **Score de Risco**, realizei uma comparação de performance entre quatro algoritmos. O **Gradient Boosting** destacou-se pela sua capacidade de corrigir erros sequencialmente durante o treino.

| Modelo | Acurácia (Taxa de Acerto) | Perfil do Score |
| :--- | :---: | :--- |
| **Gradient Boosting** | **62.25%** | **Equilibrado e Preciso** |
| Regressão Logística | 62.17% | Suave e Linear |
| Random Forest | 55.32% | Tendência a Extremos |
| Árvore de Decisão | 53.46% | Radical (0 ou 100) |

---

## 💡 Insights Estratégicos (Feature Importance)
Utilizando o modelo campeão, foi possível identificar os fatores que mais "pesam" na balança do risco:

1. **Impacto do Produto:** O produto `GTX Basic` é o fator isolado de maior influência (~7.6%).
2. **Setores Chave:** Leads dos setores de **Tecnologia, Software e Entretenimento** apresentam padrões de conversão mais previsíveis.
3. **Influência do Agente:** Vendedores como *Hayden Neloms* e *Donn Cantrell* possuem padrões de atuação que alteram significativamente o score de risco.

> [!TIP]
> **O Insight para o Gestor:** Focar o esforço da equipe em produtos de alta conversão em setores onde o modelo aponta baixo risco pode aumentar o Win Rate em até 15%.

---

## 📁 Estrutura do Repositório
* `index.ipynb`: Notebook com todo o tratamento de dados e treino dos modelos.
* `dataset/`: Dados originais do CRM (Sales Pipeline, Accounts, Products, etc).

---

## 🚀 Como Executar o Projeto
1. Instale as dependências:
   ```bash
   pip install pandas scikit-learn seaborn matplotlib
   ```
2. Execute o ficheiro `index.ipynb` para processar os dados.

> *Desenvolvido por **Karla Renata** 📍 Estudante de Ciência da Computação*
