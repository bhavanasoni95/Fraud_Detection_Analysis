# Fraud Detection Analysis

## 📌 Project Overview
This project focuses on analyzing transaction data to detect potential fraud. The analysis involves data cleaning, exploratory data analysis, handling data imbalance, and applying various machine learning models to predict fraudulent transactions.

---

## 🔑 Key Features
- Monetary value of each transaction is analyzed.
- Identification of unusually high or low transaction amounts.
- Detection of outliers indicative of potential fraud.
- Improved model accuracy in distinguishing fraudulent transactions.
- Faster response to potential fraud cases.

---

## 📊 Data Description
- **Sample Size:** 6,362,620
- **Number of Features:** 11
- **Target Variable:** `isFraud` (Binary: 0 for non-fraud, 1 for fraud)

---

## 🧹 Data Cleaning
- **Missing Values:** No missing values
- **Duplicates:** No duplicate values
- **Data Types:** Features have appropriate data types
- **Outliers:** Retained, as higher values may represent fraud
- **Imbalance:** The target variable is highly imbalanced

---

## 🔍 Exploratory Data Analysis (EDA)
- **High Class Imbalance:** Few fraud cases compared to many non-fraud cases
- **Skewed 'Amount' Feature:** Mostly small transactions, few large ones
- **Balance Shifts:** Unexpected changes may indicate fraud
- **Time Matters ('step' feature):** May reveal fraud patterns
- **Interacting Features:** Important for fraud prediction
- **Highly Correlated Features:** Some features strongly correlated
- **'Amount' & Destination Balances:** Moderate positive correlation
- **'Step' Feature:** Weak or no relationship with the target
- **Encoding:** Categorical feature `type` was label encoded

---

## 📈 Data Visualization
- Visualizations used to explore distribution and imbalance of the target
- **SMOTE** (Synthetic Minority Over-sampling Technique) applied to balance classes
- Data split into 80% training and 20% testing

---

## 🤖 Model Selection
The following machine learning models were evaluated:
- Logistic Regression
- K-Nearest Neighbors Classifier
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- XGBoost Classifier
- Gaussian Naive Bayes
- Multinomial Naive Bayes
- Bernoulli Naive Bayes
- Bagging Classifier
- AdaBoost Classifier

---

## 🔍 Interpretation
- **XGBoost** was most effective at correctly flagging fraudulent transactions.
- Some models had high accuracy but struggled to detect actual fraud.
- Trade-offs exist between catching fraud and false positives.

---

## ✅ Conclusion
The analysis indicates that machine learning models can effectively detect fraudulent transactions. **XGBoost** showed the best performance. Further feature engineering and model optimization could enhance results.

---
#
