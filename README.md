# 📉 Customer Churn Prediction with Supervised Learning for Subscription-Based Services

This project focuses on predicting customer churn using supervised machine learning models. The dataset, provided by IBM, contains demographic and behavioral information of telecom customers. The main goal is to identify patterns that indicate whether a customer is likely to leave the service, helping businesses retain customers more effectively.

---

## 🧾 Project Overview

Churn prediction is critical for subscription-based businesses. This project provides a complete data science pipeline:

- Data Preprocessing & Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Imbalanced Data Handling using SMOTE
- Model Building & Evaluation (Random Forest, XGBoost)
- Performance Visualization & Insights

---

## 📂 Dataset Details

**Source**: IBM Sample Dataset  
**Target Variable**: `Churn` (Yes/No)

### Key Columns:
- **Demographics**: Gender, Partner, Dependents
- **Account Info**: Tenure, Contract, Payment Method, Monthly & Total Charges
- **Services Used**: Internet, Streaming, Tech Support, Online Security, etc.

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- SMOTE (from imbalanced-learn)

---

## 🔍 Key Steps Performed

### ✅ Data Cleaning
- Encoding issues handled with `chardet`
- Converted `TotalCharges` to numeric
- Handled missing values and invalid entries

### 📊 Exploratory Data Analysis
- Visualized churn distribution
- Compared churn rates across contract types, tenure, and services
- Found strong correlation between short tenure and churn

### ⚙️ Feature Engineering
- Label and one-hot encoding for categorical variables
- Feature scaling using `StandardScaler`

### 🧠 Model Building
- **Random Forest Classifier**
- **XGBoost Classifier**
- GridSearchCV used for hyperparameter tuning

### 📈 Evaluation Metrics
- Accuracy
- Confusion Matrix
- ROC Curve & AUC Score
- Precision-Recall Curve

---

## 💡 Business Insights

- **Short Tenure = High Churn**: Customers in their early months are more likely to churn. Early engagement and onboarding strategies are crucial.
- **Contract Type Matters**: Month-to-month contracts have significantly higher churn rates. Annual or two-year contracts show better customer retention.
- **Additional Services Improve Retention**: Customers who subscribe to multiple services (e.g., online backup, tech support) are less likely to churn.
- **Paperless Billing & Electronic Payment**: Customers using paperless billing and electronic payment methods had slightly higher churn rates. A better UX around billing might help.
- **Senior Citizens and Churn**: Senior citizens churn at a higher rate — possibly due to service complexity or pricing.

---

## 📊 Results Summary

| Model               | Accuracy | AUC Score |
|--------------------|----------|-----------|
| Random Forest       | High     | Good      |
| XGBoost             | High     | Excellent |

- **SMOTE** improved recall by balancing the class distribution.
- **XGBoost** achieved the best overall performance.

---
