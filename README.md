# Credit Card Fraud Detection Analysis

## Project Overview
This project focuses on **detecting fraudulent credit card transactions** using machine learning techniques. Fraud detection is critical in financial systems to minimize losses and protect customers. The project compares the performance of **Logistic Regression** and **XGBoost Classifier** to identify the most effective model.

---

## Dataset
- **Source:** [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Size:** 284,807 transactions  
- **Features:**  
  - `V1` to `V28` — PCA-transformed anonymized features  
  - `Amount` — Transaction amount  
  - `Class` — Target variable (0 = Non-Fraud, 1 = Fraud)  

---


---

## Steps Performed

### 1. Data Loading
- Loaded the dataset and explored basic information and missing values.

### 2. Exploratory Data Analysis (EDA)
- Checked distribution of fraud vs non-fraud transactions.
- Visualized correlations and feature distributions.
- Identified class imbalance.

### 3. Data Preprocessing
- Scaled the `Amount` feature.
- Handled class imbalance using **SMOTE**.
- Split data into training and test sets.

### 4. Feature Engineering (Optional)
- Added derived features (e.g., transaction hour from `Time` if available).

### 5. Model Building
- **Logistic Regression**
- **XGBoost Classifier**

### 6. Model Evaluation
- Metrics used:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
  - Confusion Matrix
- Visualized ROC curves for both models.

### 7. Feature Importance
- Identified top features contributing to fraud detection using XGBoost.

### 8. Conclusion
- Compared model performance.
- Highlighted the best-performing model.
- Provided insights and recommendations for practical deployment.

---

## Key Findings
- Fraud transactions are extremely rare (highly imbalanced dataset).
- XGBoost generally outperforms Logistic Regression in ROC-AUC and recall.
- Features `V14`, `V17`, `V12` (example) were the most important for fraud prediction.

---

## Libraries Used
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  
- imbalanced-learn (SMOTE)  
- xgboost  

---

