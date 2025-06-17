# 📊 Bank Marketing Classifier Comparison

## 🎯 Objective
This project compares the performance of four machine learning classifiers—Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree, and Support Vector Machine (SVM)—on the Portuguese Bank Marketing dataset. The goal is to predict whether a client will subscribe to a term deposit based on features collected during direct marketing campaigns.

## 🗃️ Dataset
- **Source**: UCI Machine Learning Repository
- **File**: `bank-additional-full.csv`
- **Target Variable**: `y` (yes = subscribed, no = not subscribed)

## 🧪 Models Compared
- **Logistic Regression**
- **K-Nearest Neighbors**
- **Decision Tree**
- **Support Vector Machine**

All models were evaluated using:
- **Stratified Train/Test Split**
- **Standard Scaling (as needed)**
- **GridSearchCV for hyperparameter tuning**
- **5-fold Cross-validation**
- **Evaluation Metrics**: ROC-AUC, Confusion Matrix, Classification Report

## 📈 Results Summary
| Model               | ROC-AUC Score |
|--------------------|---------------|
| SVM                | 0.92          |
| Logistic Regression| 0.91          |
| Decision Tree      | 0.87          |
| KNN                | 0.84          |

> 📌 **SVM** and **Logistic Regression** performed the best, with SVM slightly outperforming in terms of ROC-AUC.

## 🔍 Key Insights
- **Cellular** contacts and **specific months** (like May) had higher success rates.
- Clients with a successful previous campaign were more likely to subscribe again.
- Economic indicators like `euribor3m` and `emp.var.rate` were influential.

