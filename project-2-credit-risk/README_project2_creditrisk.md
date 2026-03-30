# Project 2 — Credit Risk Classification

**ReDI School of Digital Integration — AI Certificate Program 2026**
Week 04 | Machine Learning — Supervised Learning

---

## Problem

Can we predict whether a bank client represents a high or low credit risk,
based on their financial and demographic data?

This is a **binary classification problem:**
- `0` = Low Risk
- `1` = High Risk

Understanding credit risk is one of the most important tasks in banking.
This project builds a simple but effective model to support that decision.

---

## Dataset

- **Source:** Kaggle — German Credit Data
- **Link:** https://www.kaggle.com/datasets/uciml/german-credit
- **Coverage:** 1,000 bank clients, 9 features
- **Key columns:** `Age`, `Sex`, `Job`, `Housing`, `Saving accounts`, `Checking account`, `Credit amount`, `Duration`, `Purpose`

> Dataset not included due to file size. Download directly from Kaggle.

---

## Approach

1. Loaded and inspected the dataset
2. Handled missing values in `Saving accounts` and `Checking account` columns
3. Created binary target variable based on credit amount and duration
4. Encoded categorical variables using LabelEncoder
5. Split data: 80% training, 20% testing
6. Trained a Logistic Regression model
7. Evaluated using accuracy, classification report, and confusion matrix

---

## Model

**Logistic Regression** (scikit-learn)
- Simple, interpretable, and widely used in credit scoring
- `max_iter=5000` to ensure full convergence

---

## Evaluation

| Metric | Result |
|--------|--------|
| Accuracy | **97%** |
| Low Risk correctly identified | 175 / 176 |
| High Risk correctly identified | 19 / 24 |
| Total misclassifications | 6 / 200 |

### Confusion Matrix

|  | Predicted Low | Predicted High |
|--|--------------|----------------|
| **Actual Low** | 175 ✅ | 1 ❌ |
| **Actual High** | 5 ❌ | 19 ✅ |

---

## Key Insights

- Clients with higher credit amounts and longer loan durations are more likely to be high risk
- Most clients (87.6%) fall into the low risk category
- The model performs well despite the class imbalance
- Logistic Regression is a strong baseline model for credit risk classification
- This type of model supports data-driven credit decision-making in banking environments

---

## Files

| File | Description |
|------|-------------|
| `credit_risk_classification.ipynb` | Full ML pipeline: data cleaning, encoding, train/test split, logistic regression, confusion matrix, and evaluation |
