# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning models.  
The dataset is highly imbalanced, so model evaluation is based on precision, recall, and F1-score instead of accuracy.

---

## 📊 Dataset
- Source: Kaggle Credit Card Fraud Dataset  
- Records: ~284,000 transactions  
- Features: 30 (PCA-transformed features V1–V28 + Time + Amount)  
- Target Variable:
  - 0 → Legitimate transaction  
  - 1 → Fraudulent transaction  

Dataset link:  
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

---

## ⚙️ Workflow
- Data cleaning (removed duplicate records)
- Feature scaling using StandardScaler
- Stratified train-test split (80/20)
- Model training:
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Random Forest Classifier
- Model evaluation using:
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

---

## 📈 Model Performance Comparison

| Model | Precision | Recall | F1-score |
|------|-----------|--------|----------|
| Logistic Regression | 0.84 | 0.579 | 0.688 |
| KNN | 0.829 | 0.716 | 0.768 |
| Random Forest | 0.972 | 0.737 | 0.838 |

---

## 🏆 Best Model
The Random Forest Classifier performed best due to:
- Highest F1-score
- Strong precision (low false positives)
- Good recall (detects most fraud cases)

---
---

## 📌 Conclusion
This project demonstrates the importance of handling imbalanced datasets in machine learning.

Although all models showed high accuracy, accuracy alone was misleading due to extreme class imbalance. Therefore, precision, recall, and F1-score were used as the main evaluation metrics.

👉 Final takeaway:  
Random Forest is the most suitable model for fraud detection in this dataset.
