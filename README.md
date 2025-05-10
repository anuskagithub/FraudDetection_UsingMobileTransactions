### Fraud Detection Using Mobile Transactions

This project focuses on detecting fraudulent transactions in mobile money operations using supervised machine learning techniques. The dataset was obtained from Kaggle and processed through data cleaning, exploratory analysis, model building, and evaluation.

# Objective
To build a machine learning model that can accurately classify whether a transaction is fraudulent based on transaction features, and deploy a working prototype with a dashboard for visualization and predictions.

# Dataset
Source: Kaggle - Mobile Money Fraud Detection

# Features:
type: Type of transaction (e.g., CASH_OUT, TRANSFER)
amount: Amount involved in the transaction
oldbalanceOrg, newbalanceOrig, oldbalanceDest, newbalanceDest: Balance before and after the transaction
isFraud: Target variable (1 for fraud, 0 for normal)

# Project Pipeline
1. Data Preprocessing
-Loaded dataset using pandas
-Handled missing values
-Encoded categorical variables using LabelEncoder
-Scaled features with StandardScaler
-Handled class imbalance using SMOTE

2. Exploratory Data Analysis (EDA)
-Distribution of fraud vs. non-fraud transactions
-Correlation heatmaps
-Insights on transaction types and their fraud likelihood

3. Model Building
-Trained multiple models:
  -Logistic Regression
  -XGBoost

-Used metrics like:
  -Accuracy
  -Confusion Matrix
  -ROC-AUC
  -Classification Report

4. Evaluation
-Compared model performance
-Identified XGBoost as the most accurate and reliable model

# Technologies Used
-Python
-Pandas, NumPy, Seaborn, Matplotlib
-Scikit-learn
-XGBoost
-Imbalanced-learn (SMOTE)

