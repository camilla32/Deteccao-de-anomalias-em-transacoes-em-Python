# 🚨 Detecção de Fraudes Bancárias com Machine Learning

Projeto de Data Science desenvolvido em Python para identificação de transações financeiras fraudulentas utilizando técnicas de Machine Learning, balanceamento de dados e análise exploratória.

---

# 📌 Sobre o Projeto

Fraudes financeiras representam um grande desafio para instituições bancárias e empresas digitais. Este projeto tem como objetivo desenvolver modelos inteligentes capazes de detectar transações suspeitas a partir de dados históricos de cartões de crédito.

O projeto utiliza:
- análise de dados;
- tratamento de desbalanceamento;
- engenharia de atributos;
- modelos supervisionados de Machine Learning;
- métricas de avaliação para classificação.

---

# 🚀 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Imbalanced-Learn (SMOTE)
- XGBoost
- Google Colab

---

# 📂 Dataset Utilizado

Dataset público de transações financeiras:

```python
https://storage.googleapis.com/download.tensorflow.org/data/creditcard.csv
```

O conjunto de dados contém:
- transações reais anonimizadas;
- classes desbalanceadas;
- coluna `Class`:
  - `0` → transação normal
  - `1` → fraude

---

# 🧠 Técnicas Aplicadas

## ✅ Pré-processamento
- normalização de dados;
- transformação logarítmica;
- padronização com `StandardScaler`.

---

## ✅ Engenharia de Atributos

Criação de novas variáveis:

```python
df["Amount_log"] = np.log1p(df["Amount"])
```

---

## ✅ Balanceamento de Dados

Aplicação de:
- Undersampling
- SMOTE (Synthetic Minority Oversampling Technique)

---

## ✅ Modelos Utilizados

### 🔹 Logistic Regression
Modelo baseline para classificação.

### 🔹 Random Forest
Modelo ensemble para melhoria da performance.

### 🔹 XGBoost
Modelo avançado para detecção de padrões complexos.

---

# 📊 Métricas de Avaliação

O projeto utiliza:
- Classification Report
- ROC Curve
- Precision-Recall Curve
- Confusion Matrix

---

# 📈 Visualizações

O sistema gera:
- curva ROC;
- curva Precision-Recall;
- matriz de confusão;
- distribuição de fraudes.

---

# 🛠️ Estrutura do Projeto

```bash
fraud-detection/
│
├── fraud_detection.ipynb
├── README.md
└── requirements.txt
```

---

# ▶️ Como Executar

## 1️⃣ Clone o repositório

```bash
git clone https://github.com/seu-usuario/fraud-detection.git
```

---

## 2️⃣ Instale as dependências

```bash
pip install pandas numpy matplotlib scikit-learn imbalanced-learn xgboost
```

---

## 3️⃣ Execute no Google Colab ou Jupyter Notebook

Abra o arquivo:

```bash
fraud_detection.ipynb
```

---

# 📌 Fluxo do Projeto

```text
Coleta de Dados
        ↓
Pré-processamento
        ↓
Feature Engineering
        ↓
Balanceamento de Classes
        ↓
Treinamento dos Modelos
        ↓
Avaliação de Performance
```

---

# 📌 Exemplo de Resultado

```python
precision    recall  f1-score   support

0       1.00      1.00      1.00
1       0.89      0.81      0.85
```

---

# 🎯 Principais Aprendizados

Durante o desenvolvimento deste projeto foram aplicados conceitos importantes de:
- Machine Learning;
- classificação desbalanceada;
- análise exploratória de dados;
- engenharia de atributos;
- avaliação de modelos;
- detecção de anomalias.

---

# 📚 Referências

- Scikit-Learn Documentation  
- TensorFlow Datasets  
- XGBoost Documentation  
- Imbalanced-Learn Documentation  

---

# 👨‍💻 Autor

Projeto desenvolvido para fins educacionais e prática em Data Science e Machine Learning.
