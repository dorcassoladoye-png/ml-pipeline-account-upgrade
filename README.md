# ml-pipeline-account-upgrade
End-to-end machine learning pipeline to predict business account upgrades using Logistic Regression. Built with Python, Scikit-learn, and Pandas.

# Business Account Upgrade Prediction

An end-to-end machine learning pipeline that predicts whether a business account will upgrade its plan, based on usage behaviour, company profile, and engagement data.

## Business Problem

A B2B software company wants to identify which accounts are likely to upgrade so the sales team can prioritise outreach and increase revenue efficiently. The model answers one question: **will this account upgrade — yes or no?**

## Dataset

- **Records:** 377 business accounts
- **Features:** 11 input columns covering company size, industry, annual revenue, product usage, support tickets, training attendance, and more
- **Target:** `Upgraded_Account` (Yes / No)

## ML Problem Type

Binary Classification — predicting one of two outcomes (upgraded or not upgraded).

## Pipeline Steps

1. Business problem definition
2. Data loading and inspection
3. Exploratory Data Analysis (EDA).
4. Missing value handling
5. Feature and target definition
6. Train/test split (80/20, stratified)
7. Preprocessing — StandardScaler + OneHotEncoder
8. Logistic Regression model training
9. Model evaluation — Accuracy, ROC-AUC, Classification Report, Confusion Matrix
10. Feature importance analysis

## Tools and Libraries

- Python
- Pandas
- Scikit-learn

## Model

**Logistic Regression** — selected as the baseline model for its suitability for binary classification and interpretability.

## Results

The model was evaluated on a held-out test set (20% of data) using accuracy, ROC-AUC, precision, recall, and F1-score.

## Limitation

The dataset is class imbalanced — only 22% of accounts upgraded. This may cause the model to underpredict upgrades. Future work could apply SMOTE or class weighting to improve recall on the minority class.

## Author

**Dorcas Soladoye**  
M.A. Data Analytics & Artificial Intelligence — Ontario Tech University  
Certified Business Data Analyst (CBDA®)
