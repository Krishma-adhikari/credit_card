# 💳 Credit Card Fraud Detection | Machine Learning Classification Project

## 📌 Project Overview
This project compares multiple machine learning models to detect fraudulent credit card transactions using a real-world highly imbalanced dataset.

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

## 🛠️ Tech Stack
- Python  
- Pandas  
- Scikit-learn  
- Plotly  
- Kaleido  

---

## ⚙️ Workflow
- Data cleaning (removed duplicate records)
- Feature scaling using StandardScaler
- Train-test split (80/20, stratified to handle class imbalance)
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
Random Forest Classifier performed best due to:
- Highest F1-score
- Strong precision (low false positives)
- Good recall (detects most fraud cases)

---

## 📌 Conclusion
This project demonstrates the importance of handling imbalanced datasets in machine learning.

Although all models achieved high accuracy, accuracy alone is misleading due to class imbalance.  
Therefore, precision, recall, and F1-score were used for evaluation.

👉 Final takeaway:  
Random Forest is the most suitable model for credit card fraud detection.
