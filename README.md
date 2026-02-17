# 🧠 Chronic Kidney Disease Prediction using Machine Learning

## 📌 Problem Statement
The hospital management requires a predictive model to identify whether a patient is likely to have Chronic Kidney Disease (CKD) based on several medical parameters.

---

## 📊 Dataset Information
- Dataset Name: Chronic Kidney Disease Dataset
- Number of Rows: 399
- Number of Columns: 29
- Target Variable: classification_yes

### Numerical Features
age, bp, al, su, bgr, bu, sc, sod, pot, hrmo, pcv, wc, rc

### Categorical Features
sg, rbc, pc, pcc, ba, htn, dm, cad, appet, pe, ane

---

## 🛠️ Preprocessing Steps
- Converted categorical features using One-Hot Encoding
- Split dataset into training and testing sets
- Applied GridSearchCV for hyperparameter tuning

---

## 🤖 Models Used
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Naive Bayes

---

## 📈 Model Evaluation

| Model | Accuracy | ROC AUC |
|------|----------|--------|
| Logistic Regression | 99% | 0.999 |
| SVM | 99% | 1.0 |
| Random Forest | 98% | 0.986 |
| Decision Tree | 97% | 0.975 |
| Naive Bayes | 98% | 1.0 |
| KNN | 79% | 0.84 |

---

## 🏆 Final Model Selection

Logistic Regression is selected as the final model because:
- Provides very high accuracy (99%)
- Simple and interpretable
- Suitable for medical decision-making
- Less risk of overfitting compared to SVM

---

## 🚀 Deployment

The trained model is saved using **pickle** and deployed using a Python script that accepts user inputs and predicts CKD.

---

## 📂 Project Structure

CKD-Prediction-ML-Project/
│
├── CKD.csv
├── Logistic Regression-Phase1.ipynb
├── LogReg-Phase2.py
├── finalized_model_LogReg.sav
├── model_columns.pkl
├── CKD_Document.pdf
└── README.md
