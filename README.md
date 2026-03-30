# 🏥 ICU Patient Risk Stratification

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Project-Completed-success)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Overview
In Intensive Care Units (ICUs), early decision-making is critical. Doctors must quickly assess:
- Risk of patient mortality  
- Expected ICU length of stay  

This project leverages **Machine Learning** to predict these outcomes using patient data collected within the **first 24 hours of ICU admission**.

---

## 🎯 Objectives
- Predict **hospital mortality** (Classification)
- Estimate **ICU length of stay** (Regression)
- Enable early risk assessment using ML
- Support data-driven clinical decision-making

---

## 📂 Dataset
- `training_v2.csv` — Main dataset  
- `WiDS Datathon 2020 Dictionary.csv` — Feature descriptions  

### Features Include:
- Vital signs  
- Lab results  
- Demographics  
- ICU admission details  

---

## ⚙️ Tech Stack
- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn**

---

## 🧠 Workflow

### 1. Data Preprocessing
- Cleaned column names  
- Handled missing values using **median imputation**  
- One-hot encoding for categorical variables  
- Feature scaling using **StandardScaler**  

### 2. Feature Engineering
- Removed target leakage by dropping:
  - `hospital_death`
  - `pre_icu_los_days`

---

## 🤖 Models Used

### 🔹 Classification (Mortality Prediction)
- Logistic Regression  
- Random Forest Classifier  

### 🔹 Regression (Length of Stay Prediction)
- Linear Regression  

---

## 📊 Evaluation Metrics

### Classification
- Accuracy  
- ROC-AUC Score  

### Regression
- RMSE (Root Mean Squared Error)  

---

## 📈 Results
- Random Forest outperformed Logistic Regression in mortality prediction  
- Identified key clinical indicators affecting survival  
- Regression model provided baseline ICU stay predictions  

---

### ⚠️ Limitations
- No hyperparameter tuning performed
- No cross-validation applied
- Class imbalance not addressed
- Regression target is basic approximation
- Not production-ready

---

### 📌 Future Scope
- Real-time ICU risk prediction system
- Integration with hospital data pipelines
- Explainable AI for clinical adoption
- Deployment as a decision-support system

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/ICU-Patient-Risk-Stratification.git

# Navigate into the directory
cd ICU-Patient-Risk-Stratification

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook ICU_Risk_Stratisfaction_.ipynb

ICU-Patient-Risk-Stratification/
│
├── data/
│   ├── training_v2.csv
│   └── WiDS Datathon 2020 Dictionary.csv
│
├── notebooks/
│   └── ICU_Risk_Stratisfaction_.ipynb
│
├── requirements.txt
└── README.md
```
---
## 👤 Author
Ayush & Siddhant
Computer Science Student 

---
