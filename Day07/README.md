# 📡 Project 7: Feature Engineering for Customer Churn Prediction

## 📌 Project Overview
This project focuses on **predicting customer churn** for a telecommunications company by demonstrating the **power of feature engineering** and the **art of feature selection** in machine learning.

Instead of relying only on model complexity, this project emphasizes **improving data representation** to enhance model performance—especially for the **minority churn class**, which is critical in real-world business scenarios.

---

## 🎯 Project Objective
- Build a **baseline churn prediction model** using raw features
- Design and evaluate **engineered features** using domain knowledge
- Compare model performance before and after feature engineering
- Experiment with **feature selection techniques**
- Analyze why certain methods improve (or fail to improve) performance
- Focus on improving **F1-score for churned customers (Churn = 1)**

---

## 🧠 Core Concepts Covered
- Importance of Feature Engineering
- Advanced Data Cleaning (real-world inconsistencies)
- Feature Creation Techniques:
  - Binning / Discretization (Tenure Groups)
  - Feature Aggregation (Number of services)
  - Feature Interaction (Charge ratios)
  - Category Simplification
- End-to-End ML Pipelines using `ColumnTransformer`
- Model Evaluation with Imbalanced Data
- Feature Importance & Feature Selection
- Comparative Model Analysis

---

## 📂 Dataset
- **Telco Customer Churn Dataset**
- ~7,000 customers
- Mix of numerical & categorical features
- Binary target variable: `Churn (Yes / No)`

---

## 🛠️ Tech Stack & Libraries
- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn**
  - Logistic Regression
  - Random Forest
  - Pipelines & Transformers
  - Feature Selection utilities

---

## ⚙️ Project Workflow

### 1️⃣ Data Cleaning & Preparation
- Converted incorrect data types (`TotalCharges`)
- Handled missing values
- Encoded target variable
- Verified dataset integrity

---

### 2️⃣ Baseline Model (No Feature Engineering)
- Model: **Logistic Regression**
- Preprocessing:
  - Standard Scaling (Numerical)
  - One-Hot Encoding (Categorical)
- Purpose: Create a **benchmark** for comparison

**Baseline Results (Churn Class):**
- F1-score ≈ **0.60**
- Accuracy ≈ **80%**

---

### 3️⃣ Feature Engineering (Core Improvement)
New features created using domain understanding:
- **Tenure_Group:** Binned customer tenure
- **num_add_services:** Count of subscribed add-on services
- **monthly_charge_ratio:** Monthly charges adjusted by tenure
- Simplified service categories (`No internet service → No`)

---

### 4️⃣ Enhanced Model (With Engineered Features)
- Same model (Logistic Regression) for fair comparison
- Used enriched feature set

**Enhanced Results:**
- Improved churn prediction capability
- Better balance between precision & recall
- Demonstrated that **feature quality > model complexity**

---

### 5️⃣ Feature Importance Analysis
- Trained a **Random Forest** to extract feature importances
- Visualized top contributing features
- Identified which engineered features carried the most signal

---

### 6️⃣ Feature Selection Experiment
- Method: `SelectFromModel` with Random Forest
- Threshold: Median feature importance
- Goal: Reduce dimensionality and test performance impact

**Observation:**
- Feature selection **did not improve performance** in this case
- Demonstrated that feature selection is **context-dependent**

---

## 📊 Final Performance Summary

| Model | Accuracy | F1-Score (Churn) |
|------|---------|------------------|
| Baseline Model | ~0.80 | ~0.60 |
| Enhanced Model | ~0.81 | ~0.59 |
| Selected Features Model | ~0.81 | ~0.59 |

> 📌 Key Insight:  
> Feature engineering improved churn detection, but aggressive feature selection removed useful signals for this dataset.

---

## 🔍 Key Learnings
- **Feature Engineering is critical** and often more impactful than model tuning
- **F1-score is more meaningful than accuracy** for imbalanced datasets
- Feature selection must be tested carefully—more features ≠ worse performance
- Domain knowledge plays a major role in predictive success

---

## 🚀 Future Improvements
- Try advanced models (XGBoost, LightGBM)
- Hyperparameter tuning using GridSearchCV
- SMOTE or cost-sensitive learning for class imbalance
- SHAP values for better explainability
- Deploy as a churn prediction API

---


## 📌 Conclusion
This project proves that **better data representation leads to better models**.  
By focusing on **feature engineering, thoughtful experimentation, and proper evaluation**, we can build more effective and business-aligned machine learning solutions.

---

📂 *Part of: 21 Days – 21 Machine Learning Projects*  
📈 *Day 7: Feature Engineering for Customer Churn Prediction*
