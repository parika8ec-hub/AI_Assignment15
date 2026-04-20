# Loan Default Prediction with Fairness & Explainability Analysis

## Project Overview

This project focuses on building a Machine Learning model to predict loan default risk using a bank dataset. Along with prediction, the project emphasizes Ethical AI practices, including fairness evaluation and model explainability.

The goal is not only to achieve high accuracy but also to ensure that the model behaves fairly across different demographic groups (e.g., education levels).

---

## Objectives

* Perform Exploratory Data Analysis (EDA)
* Preprocess and clean the dataset
* Train a Logistic Regression model
* Evaluate model performance
* Conduct fairness analysis across education groups
* Apply explainability techniques (SHAP & LIME)

---

## Dataset Description

The dataset contains financial and demographic features such as:

* `age` – Age of the individual
* `ed` – Education level (1–5)
* `employ` – Years of employment
* `address` – Years at current address
* `income` – Annual income
* `debtinc` – Debt-to-income ratio
* `creddebt` – Credit card debt
* `othdebt` – Other debts
* `default` – Target variable (1 = Default, 0 = No Default)

---

## Project Workflow

### 1. Data Preprocessing

* Handled missing values
* Encoded categorical variables
* Scaled numerical features using StandardScaler

> Note: Original (unscaled) data is preserved for fairness analysis.

---

### 2. Model Training

* Algorithm: Logistic Regression
* Data split into 80% training and 20% testing sets
* Model trained on scaled features

---

### 3. Model Evaluation

* Accuracy score used as primary metric
* Predictions generated on test data

---

### 4. Fairness Analysis

* Evaluated model performance across education groups
* Metrics analyzed:

  * Accuracy per group
  * Selection rate (prediction rate)

> Fairness evaluation is done using original education values for interpretability.

---

### 5. Explainability

* SHAP (SHapley Additive Explanations) for global and local feature importance
* LIME (Local Interpretable Model-agnostic Explanations) for individual predictions

---

## Key Insights

* Model achieves strong overall accuracy
* Performance varies across education groups, indicating potential bias
* Features like income and debt significantly influence predictions
* Explainability tools help understand model decisions

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/parika8ec-hub/AI_Assignment15.git
cd AI_Assignment15
```

---

### 2. Install Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn shap lime fairlearn
```

---

### 4. Run the Project using Jupyter Notebook:

```bash

Open the notebook file Assignment15.ipynb and run all cells.
```

---

## Project Structure

```
├── data/
│   └── bank-loan.csv
├── notebooks/
│   └── Assignment15.ipynb
└── README.md
```

---

## Ethical Considerations

* Bias detected across education levels
* Important to ensure fair decision-making in financial systems
* Model should not disadvantage specific groups

---

## Future Improvements

* Apply bias mitigation techniques
* Use more advanced models (e.g., Random Forest, XGBoost)
* Improve feature engineering
* Deploy model as a web application

---
