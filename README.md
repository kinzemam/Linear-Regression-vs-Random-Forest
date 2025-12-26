# 🧬 Breast Cancer Classification using Machine Learning

## 📌 Project Overview
This project focuses on classifying breast cancer tumors as **benign** or **malignant** using machine learning classification models.  
The primary objective is to **compare model performance** using appropriate evaluation metrics and to analyze the effect of **threshold tuning** in a medical classification context.

No exploratory data analysis (EDA) is performed in this project. The emphasis is strictly on **model training, evaluation, and comparison**.

---

## 📊 Dataset
- Breast Cancer dataset containing diagnostic features
- Target variable:
  - `0` → Benign  
  - `1` → Malignant  

---

## 🧠 Models Implemented

### 1️⃣ Logistic Regression
- Features scaled using **StandardScaler**
- Probabilistic predictions generated using `predict_proba`
- **Decision threshold tuned to 0.5** to prioritize recall and reduce false negatives

### 2️⃣ Random Forest Classifier
- Ensemble-based, non-linear classifier
- No feature scaling required
- Used as a benchmark model for comparison

---

## 📈 Model Evaluation
The models were evaluated using the following metrics:
- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-score
- Classification Report

### Evaluation Focus
In medical diagnosis tasks, **minimizing false negatives** is critical.  
Therefore, special attention was given to **recall for the malignant class**, even at the cost of a slight increase in false positives.

---

## 📊 Model Comparison Summary

| Model | Accuracy | Recall (Malignant) | F1-score |
|------|----------|--------------------|----------|
| Logistic Regression (threshold = 0.3) | High | Higher | High |
| Random Forest | High | Slightly Lower | High |

Logistic Regression demonstrated improved recall after threshold tuning, making it more suitable for this medical classification task.

---

📈 ROC–AUC Analysis

-ROC curves are plotted for both Logistic Regression and Random Forest
-AUC scores are computed using predicted probabilities
-This helps in understanding model performance across different threshold values

---

## 🧪 Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## 🏁 Conclusion
This project demonstrates how **model choice and decision threshold selection** significantly impact performance in medical classification problems.  
Logistic Regression, when combined with feature scaling and threshold tuning, provided strong and interpretable results compared to Random Forest.

---

## 📌 Future Improvements
- Precision–Recall curve analysis
- Hyperparameter tuning
- Evaluation of additional classifiers (KNN, SVM)

---

## 👤 Author
**Md Inzemam Khan**  
B.Tech (ECE) | Machine Learning Enthusiast
