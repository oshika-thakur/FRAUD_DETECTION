# 💳 Credit Card Fraud Detection

A machine learning project that detects fraudulent transactions from credit card data.  
This project demonstrates end-to-end handling of **imbalanced classification problems**, including data preprocessing, oversampling (SMOTE), model building, and evaluation.

---

## 📌 Overview
Credit card fraud is a major financial threat worldwide. Detecting fraudulent transactions in real-time is challenging due to:
- Highly imbalanced data (frauds are <1% of total transactions).
- Trade-off between catching frauds (recall) and avoiding false alarms (precision).

This project builds classification models to detect fraud, focusing on **recall** (catching frauds) while maintaining reasonable precision.

---

## 📂 Dataset
- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Rows:** ~285,000  
- **Fraudulent transactions:** ~0.17%  
- **Features:** 30 (V1–V28 anonymized PCA features, `Time`, `Amount`, and `Class` as target)

---

## ⚙️ Features & Workflow
1. **Exploratory Data Analysis (EDA)**
   - Data shape, missing values, class imbalance visualization.
2. **Data Preprocessing**
   - Standardization of `Amount` feature.
   - Train-test split.
3. **Handling Imbalance**
   - Applied **SMOTE** to oversample the minority class.
4. **Modeling**
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier
5. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1-score
   - Special focus on **Recall**, since missing fraud is more costly than false positives.

---

## 📊 Results
- **Logistic Regression**: Good baseline, interpretable.  
- **Decision Tree**: Captures non-linear patterns but prone to overfitting.  
- **Random Forest**: Best overall performance with strong recall and balanced precision.  


