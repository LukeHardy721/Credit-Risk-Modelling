# Credit Risk Modelling with LendingClub Data

This project aims to build a machine learning model to assess credit risk using publicly available LendingClub loan data. The goal is to predict whether a loan will default, helping lenders make better risk-based decisions.

## 📊 Dataset

- **Source**: [LendingClub Loan Data](https://www.kaggle.com/datasets/wordsforthewise/lending-club/data)
- **Size**: 2,260,701 x 151
- **Data Type**: Historical loan data (e.g., loan amount, term, interest rate, grade, employment, etc.)
- **Target Variable**: `loan_status` — used to define whether a loan is "good" or "bad"

---

## 💡 Objective

To develop a **binary classification model** that predicts whether a loan will default based on borrower and loan characteristics.

---

## 🧰 Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🧪 Workflow

1. **Data Preparation**
   - Basic data cleaning
   - Drop irrelevant or leakage features
2. **EDA & Preprocessing**
   - Explore features
   - Analye relationships with the target
   - Create new features (e.g., `debt_to_income`)
   - Impute missing values
   - Encode categorical variables
3. **Modelling - Logistic Regression**
   - Analyse collinearity
   - PCA
   - SMOTE
   - Stochastic Gradient Descent
   - Evaluate with AUC, F1 score, precision, recall
4. **Modelling - Random Forest & XGBoost**
   - Random Forest
   - XGBoost
   - Evaluate with AUC, F1 score, precision, recall
---

## 📈 Results

| Model              | AUC Score | F1 Score | PR AUC |
|--------------------|-----------|----------|--------|
| LogisticRegression | 0.71      | 0.70     | 0.38   |
| RandomForest       | 0.72      | 0.72     | 0.39   |
| XGBoost            | 0.74      | 0.70     | 0.41   |

*(Results will vary depending on hyperparameters and train/test split)*

---

## 📂 Project Structure

```bash
credit-risk-model/
├── data/                   # Raw and processed data (excluded via .gitignore)
├── notebooks/              # Jupyter notebooks for data preparation, cleaning & EDA, and modelling
├── LCDataDictionary.xlsx   # Data dictionary
├── README.md
└── .gitignore