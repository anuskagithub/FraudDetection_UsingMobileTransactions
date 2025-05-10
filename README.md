# Fraud Detection Using Mobile Transactions

This project focuses on detecting fraudulent transactions in mobile money operations using supervised machine learning techniques. The dataset was obtained from Kaggle and processed through data cleaning, exploratory analysis, model building, and evaluation.

# Objective
To build a machine learning model that can accurately classify whether a transaction is fraudulent based on transaction features, and deploy a working prototype with a dashboard for visualization and predictions.

# Dataset
Source: [Kaggle - Mobile Money Fraud Detection](https://www.kaggle.com/code/gcdatkin/mobile-payment-fraud-detection)

# Features:
type: Type of transaction (e.g., CASH_OUT, TRANSFER)
amount: Amount involved in the transaction
oldbalanceOrg, newbalanceOrig, oldbalanceDest, newbalanceDest: Balance before and after the transaction
isFraud: Target variable (1 for fraud, 0 for normal)

# Project Pipeline
1. Data Preprocessing
- Loaded dataset using pandas
- Handled missing values
- Encoded categorical variables using LabelEncoder
- Scaled features with StandardScaler
- Handled class imbalance using SMOTE

2. Exploratory Data Analysis (EDA)
- Distribution of fraud vs. non-fraud transactions
- Correlation heatmaps
- Insights on transaction types and their fraud likelihood

3. Model Building
- Trained multiple models:
  - Logistic Regression
  - XGBoost

- Used metrics like:
  - Accuracy
  - Confusion Matrix
  - ROC-AUC
  - Classification Report

4. Evaluation
- Compared model performance
- Identified XGBoost as the most accurate and reliable model

# Technologies Used
- Python
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)

## Demo: Output Screenshots
Here are the snapshots of the project outputs:

### 1. EDA - Fraud vs Non-Fraud Transaction Count
<img width="343" alt="image" src="https://github.com/user-attachments/assets/b497adab-8564-46dd-93bb-801c2a54b772" />

### 2.Transaction Amount Distribution: Fraud vs Non-Fraud
<img width="509" alt="image" src="https://github.com/user-attachments/assets/8fa21a50-ff56-4ce8-b3aa-96a0748284de" />

### 3.Fraud Count Across Transaction Types
<img width="527" alt="image" src="https://github.com/user-attachments/assets/717bc48c-4af4-4e78-9517-6b2416e7f72b" />

### 4. Correlation Heatmap
<img width="376" alt="image" src="https://github.com/user-attachments/assets/5a539ae1-a3d5-422d-872f-7385c92bc138" />

### 5. ROC-Curve
<img width="468" alt="image" src="https://github.com/user-attachments/assets/02ab6487-371e-429f-a324-f2fb7bcf87a3" />






