# 📊 Análise Estatística e Risco de Inadimplência

Este projeto realiza uma **análise estatística aplicada** para compreender o risco de inadimplência de clientes utilizando o dataset **Default of Credit Card Clients (UCI)**.  
O foco do estudo é identificar **padrões, associações e evidências estatísticas** que expliquem a inadimplência **antes da adoção de modelos preditivos mais complexos**.

A abordagem prioriza **explicabilidade, rigor estatístico e interpretação orientada ao negócio**, servindo como base para decisões de crédito e análises futuras.

---

## 🧠 Contexto

Instituições financeiras lidam diariamente com o desafio de conceder crédito de forma equilibrada, minimizando risco sem comprometer crescimento.  
Neste projeto, a inadimplência é analisada sob a ótica estatística, buscando responder perguntas como:

- Existem diferenças estatisticamente significativas entre clientes inadimplentes e não inadimplentes?
- É possível quantificar o risco com base em evidências observáveis?
- Quais variáveis apresentam maior associação com inadimplência?

---

## 📂 Conjunto de Dados

**Fonte:** UCI Machine Learning Repository — *Default of Credit Card Clients*

O dataset contém informações financeiras, demográficas e histórico de pagamento de clientes, incluindo:

- **Variável alvo**
  - `DEFAULT`: indicador de inadimplência (0 = não inadimplente, 1 = inadimplente)
- **Capacidade financeira (proxy)**
  - `LIMIT_BAL` — limite de crédito
- **Perfil demográfico**
  - `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`
- **Histórico de pagamento**
  - `PAY_0`, `PAY_2`, `PAY_3`, `PAY_4`, `PAY_5`, `PAY_6`
- **Faturas e pagamentos**
  - `BILL_AMT1..6`, `PAY_AMT1..6`

> **Nota:** como a renda não está disponível no dataset, o `LIMIT_BAL` foi utilizado como **proxy de capacidade financeira**.

---

## 🎯 Objetivos

- Caracterizar o perfil estatístico de clientes inadimplentes e não inadimplentes  
- Estimar probabilidades marginais e condicionais de inadimplência  
- Avaliar padrões por meio de distribuições estatísticas  
- Construir intervalos de confiança para médias e proporções  
- Realizar testes de hipóteses para validar diferenças entre grupos  
- Gerar insights explicáveis para apoiar decisões de crédito  

---

## 🧪 Metodologia

O projeto foi estruturado em etapas estatísticas progressivas:

### 🔹 ETAPA 1 — Estatística Descritiva
- Média, mediana e moda  
- Variância, desvio padrão, quartis e IQR  
- Correlação de Pearson  
- Comparação entre inadimplentes e não inadimplentes  

### 🔹 ETAPA 2 — Probabilidade
- Probabilidade marginal de inadimplência  
- Probabilidades condicionais com base em evidências  
- Regra do Produto  
- Regra de Bayes  

### 🔹 ETAPA 3 — Distribuições Estatísticas
- Distribuição Normal (variáveis contínuas)  
- Distribuição Binomial/Bernoulli (inadimplência)  
- Distribuição de Poisson (eventos de atraso)  

### 🔹 ETAPA 4 — Inferência Estatística
- Intervalos de confiança para médias  
- Intervalos de confiança para proporções  
- Interpretação da incerteza estatística  

### 🔹 ETAPA 5 — Testes de Hipóteses
- Teste t (Welch) para comparação de médias  
- Teste Qui-quadrado para associação entre variáveis categóricas  
- ANOVA (quando aplicável)  

---

## 📌 Principais Resultados

- Clientes inadimplentes apresentaram **menor limite de crédito médio**, indicando associação entre capacidade financeira (proxy) e inadimplência  
- Diferenças na **dispersão de idade** foram observadas entre os grupos  
- Variáveis relacionadas ao **histórico de pagamento** mostraram associação mais consistente com inadimplência do que variáveis demográficas isoladas  
- Testes estatísticos forneceram evidências formais que sustentam as diferenças observadas  

---

## 💡 Insights de Negócio

- Histórico de pagamento é um forte indicador de risco  
- Medidas estatísticas simples e explicáveis podem apoiar políticas de concessão e monitoramento de crédito  
- A análise estatística fornece base sólida antes da aplicação de modelos preditivos mais complexos  

---

## 🛠️ Tecnologias Utilizadas

- Python  
- Pandas  
- NumPy  
- SciPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  
