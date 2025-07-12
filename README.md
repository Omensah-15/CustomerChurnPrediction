# 📉 Customer Churn Prediction with Supervised Learning for Subscription-Based Services

A supervised machine learning project to predict customer churn based on demographic, service usage, and account information. This solution is designed to support strategic retention efforts by identifying at-risk customers.

---

## 📚 About the Dataset

**Source:** [IBM Sample Data Sets]  
Each row in the dataset represents a unique customer, and each column contains attributes related to customer demographics, services subscribed, and account information.

### Dataset Includes:
- **Churn Status:** Whether the customer left in the last month (`Yes` or `No`)
- **Services:** Phone, Internet, Online Security, Backup, Tech Support, Streaming
- **Account Info:** Tenure, Contract Type, Billing Method, Monthly & Total Charges
- **Demographics:** Gender, Senior Citizen, Partner, Dependent status

---

## 🎯 Project Objective

To analyze customer data and build machine learning models that can:
- Predict the likelihood of a customer churning
- Support the development of targeted customer retention programs

---

## 🔍 Exploratory Data Analysis (EDA)

- **Churn Distribution:**
  - Customers Not Churned: `5174`
  - Customers Churned: `1869`

This indicates that around **26.5%** of customers in the dataset churned, highlighting a significant churn rate worth addressing.

- **Key Patterns Identified:**
  - Customers with month-to-month contracts, higher monthly charges, or paperless billing were more likely to churn.
  - Long-tenured customers and those on yearly contracts showed higher loyalty.
  - Services like tech support and online security were associated with reduced churn rates.

---

## 🧠 Model Building

Multiple models were tested. The final model was trained using a **Random Forest Classifier** due to its superior performance in handling imbalanced data and feature importance ranking.

### 📊 Confusion Matrix
Confusion Matrix:
[[939  94]
 [193 181]]


### ✅ Evaluation Metrics

| Metric         | Class 0 (Not Churned) | Class 1 (Churned) |
|----------------|-----------------------|--------------------|
| Precision      | 0.83                  | 0.66               |
| Recall         | 0.91                  | 0.48               |
| F1-score       | 0.87                  | 0.56               |

- **Overall Accuracy:** 80%
- **Macro F1-Score:** 71%
- **Insight:** The model performs well in identifying non-churning customers but needs further optimization (e.g., SMOTE, cost-sensitive learning) to improve recall for churning customers.

---

## 💡 Business Insights

- **Customer Retention Risk:** Nearly 1 in 4 customers are at risk of churn, with strong indicators being short tenure, monthly contracts, and high billing charges.
- **Loyalty Indicators:** Long-term contracts, additional services (security, tech support), and lower monthly costs contribute to customer retention.
- **Actionable Strategy:**
  - Provide retention offers for customers on monthly contracts.
  - Promote bundle services and annual contracts.
  - Improve onboarding for new customers to reduce early churn.

---

## 🛠️ Tools & Technologies

- **Languages & Libraries:** Python, Pandas, NumPy, Seaborn, Scikit-learn, Matplotlib
- **Environment:** Jupyter Notebook

---


