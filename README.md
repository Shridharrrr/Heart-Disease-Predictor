# 🧠 Heart Disease Risk Predictor – Bayesian Network Approach

Welcome to **MediMystery Labs**, where you're the **Data Detective** tasked with predicting heart disease risk using a Bayesian Network trained on simulated patient data.

---

## 📊 Project Overview

This project analyzes a heart disease dataset using a **Bayesian Network** (via `pgmpy`) to:
- Clean and normalize patient data
- Build a probabilistic model from a defined structure
- Train the model using **Maximum Likelihood Estimation**
- Run health-related queries like:  
  ➤ _What's the probability of heart disease given a certain age?_  
  ➤ _What's the cholesterol distribution among at-risk patients?_

---

## 🔧 Features

- Removes duplicates and missing values
- Applies Min-Max normalization to numerical data
- Converts continuous features into discrete bins (for Bayesian modeling)
- Builds a Bayesian Network with structure:
```

age → fbs → target → chol, thalach

````
- Answers diagnostic queries using `VariableElimination` inference

---

## 🛠️ Installation

Install dependencies using pip:

```bash
pip install pandas scikit-learn pgmpy
````

> If you face issues with `pgmpy`, try:

```bash
pip install git+https://github.com/pgmpy/pgmpy
```


## 🧪 Sample Diagnostic Questions

* `P(Heart Disease | Age ≈ 0.6)`
* `Cholesterol Distribution | target = 1 and thalach > 0.8`
* Custom evidence-based queries using the trained model

---
