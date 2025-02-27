# 📌 Machine Learning e Inferência Causal para Estratégias de Cobrança

Este projeto tem como objetivo utilizar **Ciência de Dados e Inferência Causal** para analisar estratégias de cobrança e melhorar a taxa de pagamento de mensalidades.

## 📂 Estrutura do Projeto

O projeto está dividido em **duas partes principais**:

### **1️⃣ Tarefa 1: Machine Learning para Predição de Pagamento**
- **Objetivo:** Prever a probabilidade de um aluno pagar sua mensalidade após uma ação de cobrança.
- **Abordagem:**
  - Análise exploratória e tratamento de dados.
  - Criação de novas features relevantes.
  - Treinamento de modelos preditivos (**Random Forest** foi o escolhido).
  - Avaliação do modelo com métricas como **Acurácia, ROC AUC, Matriz de Confusão**.
- **Saída:** Probabilidade de pagamento para cada aluno.

### **2️⃣ Tarefa 2: Inferência Causal para Avaliação das Estratégias de Cobrança**
- **Objetivo:** Determinar se as cobranças via **WhatsApp, E-mail e SMS** causam um aumento real na taxa de pagamento.
- **Abordagem:**
  - Uso de **Propensity Score Matching (PSM)** para criar grupos comparáveis.
  - Aplicação de **Regressão OLS** para estimar impacto causal.
  - Comparação de taxas de pagamento entre grupo tratado e grupo controle.
- **Conclusão:** Nenhuma das cobranças teve impacto significativo na taxa de pagamento. Recomendamos **testar novas abordagens** por meio de um **experimento A/B**.

---

## 🚀 Como Executar o Projeto

### 1️⃣ **Clone o repositório**
bash
git clone https://github.com/lucasodl95/MLeInferenciaCausal
cd seu-repositorio


### 2️⃣ **Crie um ambiente virtual e instale as dependências**
bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
pip install -r requirements.txt


### 3️⃣ **Execute o notebook**
Abra e rode os notebooks referentes às tarefas **1 (Predição) e 2 (Inferência Causal)**.

---

## 📦 Dependências
As bibliotecas necessárias estão listadas no **requirements.txt**. Principais pacotes:
- pandas
- numpy
- seaborn
- scikit-learn
- statsmodels
- matplotlib
- tqdm

---

## 📊 Resultados
- **Modelo de Machine Learning**: Acurácia de **88,4%** na predição de pagamento.
- **Inferência Causal**: Nenhuma cobrança teve efeito positivo significativo.
- **Recomendação**: Teste A/B para otimizar a estratégia de cobrança.
