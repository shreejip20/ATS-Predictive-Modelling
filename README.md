# ATS Customer Churn Prediction – Predictive Modelling

## Project Overview

This project focuses on predicting customer churn using predictive modelling techniques.

The objective is to identify customers who are likely to churn and compare different machine learning classification models based on their predictive performance.

The project uses the ATS customer dataset and treats **Churn** as the target variable.

---

## Project Objective

The main objectives of this project are:

- Predict whether a customer is likely to churn.
- Prepare and preprocess the dataset for machine learning.
- Build Logistic Regression and Random Forest classification models.
- Evaluate the models using multiple performance metrics.
- Identify the best-performing predictive model.
- Generate customer churn probabilities and risk levels.
- Provide business insights that can support customer retention strategies.

---

## Dataset

The project uses:

**Dataset:** `Dataset_ATS_v2_preprocessed.csv`

The target variable is:

**Churn**

The target represents whether a customer has churned.

---

## Methodology

The predictive modelling workflow consists of the following steps:

1. Load the ATS customer dataset.
2. Inspect the dataset structure and data quality.
3. Prepare the `Churn` target variable.
4. Separate predictor variables from the target.
5. Identify numeric and categorical features.
6. Handle missing values.
7. Standardise numeric variables.
8. Encode categorical variables.
9. Split the data into training and testing datasets.
10. Train Logistic Regression.
11. Train Random Forest.
12. Evaluate both models.
13. Compare model performance.
14. Select the preferred predictive model.
15. Generate customer churn probabilities.
16. Categorise customers into Low, Medium and High churn-risk groups.

---

## Machine Learning Models

### 1. Logistic Regression

Logistic Regression was used as a classification model to predict the probability that a customer will churn.

### 2. Random Forest

Random Forest was used as a tree-based classification model to capture potentially non-linear relationships between customer characteristics and churn.

---

## Model Performance

The models were evaluated using Accuracy, Precision, Recall, F1 Score and ROC-AUC.

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 72.94% | 49.37% | **76.54%** | **60.02%** | **81.79%** |
| Random Forest | **75.76%** | **54.34%** | 54.19% | 54.27% | 78.26% |

---

## Best Predictive Model

Based on the evaluation results, **Logistic Regression was selected as the preferred predictive model**.

Although Random Forest achieved higher Accuracy and Precision, Logistic Regression achieved:

- The highest Recall: **76.54%**
- The highest F1 Score: **60.02%**
- The highest ROC-AUC: **81.79%**

For customer churn prediction, identifying customers who are actually likely to churn is particularly important. Therefore, the higher Recall and ROC-AUC achieved by Logistic Regression make it the preferred model for this project.

---

## Business Interpretation

The predictive model can help a business identify customers who have a higher probability of leaving.

Customers can be grouped into three risk categories:

- **Low Risk:** predicted churn probability below 30%
- **Medium Risk:** predicted churn probability from 30% to below 60%
- **High Risk:** predicted churn probability of 60% or higher

High-risk customers can be prioritised for customer retention activities such as:

- Targeted retention offers
- Customer service follow-ups
- Contract or pricing reviews
- Personalised communication
- Loyalty incentives

---

## Project Outputs

The project contains:

- Predictive modelling Jupyter Notebook
- Preprocessed ATS customer dataset
- Customer churn prediction output
- Model evaluation results
- Confusion matrices
- ROC curve
- Random Forest feature importance analysis

---

## Repository Structure

```text
ATS-Predictive-Modelling/
│
├── ATS_Predictive_Modelling_TRUE_WORKING.ipynb
├── Dataset_ATS_v2_preprocessed.csv
├── ATS_customer_churn_predictions.csv
└── README.md
