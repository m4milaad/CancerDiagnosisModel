# 🧠 Breast Cancer Prediction with Machine Learning

This project is a machine learning solution for detecting breast cancer using diagnostic data. It applies data preprocessing, feature scaling, and classification models to predict whether a tumor is **benign** or **malignant**.

---

## 📁 Dataset

We use the **Breast Cancer Wisconsin (Diagnostic)** dataset. It contains features computed from digitized images of a breast mass.

- 📄 File: `Cancer_Data.csv`
- 569 records (patients)
- 32 columns: includes `id`, `diagnosis` (target), and 30 real-valued features

---

## 🔍 Objective

To develop a high-accuracy classifier using:
- Random Forest (baseline)
- XGBoost (optimized with Grid Search)

Achieved accuracy: **~99%**

---

## ⚙️ Workflow Overview

1. **Data Cleaning**
   - Dropped irrelevant columns (`id`, unnamed)
   - Encoded diagnosis: `M → 1`, `B → 0`

2. **Feature Scaling**
   - Applied `StandardScaler` for normalization

3. **Modeling**
   - Trained `RandomForestClassifier` for baseline accuracy
   - Tuned `XGBClassifier` using `GridSearchCV` for best performance

4. **Evaluation**
   - Accuracy Score
   - Classification Report
   - Confusion Matrix

---

## 📊 Results

- **Accuracy:** ~99%
- **Precision/Recall (Malignant):** High
- **Confusion Matrix:**
