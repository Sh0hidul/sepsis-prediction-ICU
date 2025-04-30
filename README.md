# 🧠 Early Prediction of Sepsis in ICU Using Machine Learning

🔗 **Live Report**: [ml_report_final.pdf](./ml_report_final.pdf)  
📁 **Notebook**: [sepsis_prediction_solution.ipynb](./notebooks/sepsis_prediction_solution.ipynb)  
📌 Course: ISAN 5367 – Texas State University (Spring 2025)

## 🚀 Project Overview

Sepsis is a critical condition that requires early intervention. In this project, we built a machine learning pipeline to predict sepsis **6 hours before onset** using ICU patient data from the **PhysioNet 2019 challenge**.

Our end-to-end ML workflow compares **13 classifiers** with **SMOTE** and **undersampling** strategies to find the most balanced model. Results showed that **XGBoost (undersampled)** performed best, with **Recall₁ = 0.84**.

---

## 🛠 Technologies Used

- **Python** (scikit-learn, XGBoost, pandas, SHAP)
- **Google Colab** (GPU-enabled)
- **SMOTE** & Random Undersampling
- **Matplotlib / Seaborn**
- **SHAP** for explainability

---

## 📊 Results Snapshot

| Model         | Recall (Non-Sepsis) | Recall (Sepsis) | Accuracy |
|---------------|----------------------|------------------|----------|
| XGBoost (Undersampled) | 0.86 | 0.84 | 0.86 |
| Tuned Random Forest     | 0.83 | 0.88 | 0.83 |
| Bagging Classifier      | 0.87 | 0.82 | 0.87 |

---

## 📁 Project Structure

```
sepsis-prediction-ICU/
├── ml_report_final.pdf                # Project summary report
├── notebooks/
│   └── sepsis_prediction_solution.ipynb
├── src/
│   ├── preprocessing.py
│   ├── modeling.py
│   └── utils.py
├── requirements.txt
└── README.md
```

---

## 📌 Key Contributions

- Used **13 ML classifiers** and **cross-validation** to benchmark model performance.
- Addressed **severe class imbalance** using SMOTE and undersampling.
- Applied **Patient_ID-level splits** to avoid data leakage.
- Achieved balanced recall between septic and non-septic classes.
- Visualized model interpretability using **SHAP** values.

---

## 📈 Future Work

- Implement time-series deep learning models (LSTM, TCN)
- Real-time deployment in ICU with edge computing
- Clinical validation with hospital data

---

## 🧑‍💻 Authors

- Shohidul Haque  
- Md Shoaib Ullash  
- Navya Kalikota  
- Siddhartha Dadireddy  
- Md Rashed Imtiouz  
- Kannammal Subramanian Palaniappan
