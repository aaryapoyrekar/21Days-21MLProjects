# 🏠 Day 03 – House Price Prediction (Regression)

## 📌 Project Overview
This project focuses on building an **end-to-end regression pipeline** to predict house sale prices using the **Ames Housing Dataset**.  
It covers the complete machine learning workflow — from exploratory data analysis and feature engineering to model training, evaluation, and Kaggle submission.

---

## 🎯 Objective
To accurately predict the **SalePrice** of houses based on multiple numerical and categorical features, and improve model performance through **feature engineering and hyperparameter tuning**.

---

## 📂 Dataset
- Source: **Kaggle – House Prices: Advanced Regression Techniques**
- Files used:
  - `train.csv`
  - `test.csv`

---

## 🔍 Exploratory Data Analysis (EDA)
- Analyzed the distribution of the target variable `SalePrice`
- Identified **positive skewness** and applied **log transformation**
- Used correlation heatmaps to identify features strongly related to price  
  (`OverallQual`, `GrLivArea`, `GarageCars`, `GarageArea`)

---

## 🛠 Data Preprocessing
- Handled missing values using:
  - Zero imputation for numerical absence-based features
  - Median imputation by neighborhood for `LotFrontage`
  - Mode / `"None"` imputation for categorical features
- Combined train and test datasets to ensure **consistent preprocessing**
- Applied **One-Hot Encoding** for categorical variables

---

## ⚙️ Feature Engineering
New features created to improve model performance:
- `TotalSF` – Total square footage
- `TotalBath` – Total number of bathrooms
- `Age` – Age of the house at the time of sale
- `RemodAge` – Years since last remodel
- `TotalPorchSF` – Total porch area
- `TotalRooms` – Total rooms including bedrooms
- `HasGarage` – Binary indicator for garage presence
- `HasBasement` – Binary indicator for basement presence

---

## 🤖 Models Used
### 1️⃣ Linear Regression (Baseline)
- Used as a simple baseline model
- Limited performance due to non-linear relationships

### 2️⃣ XGBoost Regressor (Final Model)
- Tuned hyperparameters for better generalization
- Captures complex non-linear interactions
- Significantly outperformed Linear Regression

---

## 📊 Model Evaluation Metrics
- **RMSE (Root Mean Squared Error)**
- **MAE (Mean Absolute Error)**
- **R² Score**

✔ XGBoost achieved lower error and higher R² compared to the baseline model.

---

## 📦 Submission
- Generated `submission.csv`
- Reversed log transformation before final prediction
- Successfully submitted predictions to Kaggle

---

## 🧠 Key Learnings
- Feature engineering has a major impact on model accuracy
- Log transformation helps stabilize skewed target variables
- Tree-based models perform better on complex tabular datasets
- Consistent preprocessing prevents data leakage

---

## 🚀 Future Improvements
- Hyperparameter tuning using GridSearchCV
- Advanced feature interactions
- Ensemble modeling for further performance gains

---

## ✅ Status
✔ Project Completed  
✔ Accuracy Improved  
✔ Kaggle Submission Successful  

---

📌 **Part of the series:** *21 Days – 21 Machine Learning Projects*
