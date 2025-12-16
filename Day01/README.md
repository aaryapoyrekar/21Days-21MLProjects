# 🚢 Day 01 – Exploratory Data Analysis (EDA) on Titanic Dataset

## 📌 Project Overview
This project focuses on performing **end-to-end Exploratory Data Analysis (EDA)** on the famous **Titanic dataset** to understand the key factors that influenced passenger survival during the disaster.

Instead of jumping directly into machine learning, this project emphasizes **understanding the data first** by analyzing patterns, trends, missing values, and relationships between features.

---

## 🎯 Objective
- To explore and understand the Titanic passenger dataset
- To identify important factors affecting survival
- To prepare the dataset for future machine learning modeling

---

## 🧠 What is Exploratory Data Analysis (EDA)?
Exploratory Data Analysis is the process of:
- Understanding the structure of the data
- Detecting missing values and outliers
- Studying feature distributions
- Finding relationships between variables

EDA helps in making **data-driven decisions** before building any machine learning model.

---

## 🗂️ Dataset Information
- **Dataset Name:** Titanic Dataset
- **Number of Rows:** 891
- **Number of Columns:** 12
- **Target Variable:** `Survived`

Key features include:
- `Age`, `Sex`, `Pclass`, `Fare`
- `Embarked`, `Cabin`
- `SibSp`, `Parch`

---

## 🧹 Data Cleaning & Preprocessing
The following steps were performed:
- Missing values in `Age` filled using **median**
- Missing values in `Embarked` filled using **mode**
- `Cabin` had many missing values, so a new feature **`Has_Cabin`** was created
- Verified that the cleaned dataset contains no critical missing values

---

## 📊 Exploratory Data Analysis Performed

### 🔹 Univariate Analysis
- Distribution of categorical features like `Sex`, `Pclass`, `Embarked`
- Distribution of numerical features like `Age` and `Fare`

### 🔹 Bivariate Analysis
- Survival rate by:
  - Gender
  - Passenger class
  - Age groups
  - Cabin availability
  - Port of embarkation

### 🔹 Multivariate Analysis
- Combined analysis of `Sex`, `Pclass`, and `Age` with survival
- Visualization of complex relationships using violin plots and bar plots

---

## 🛠️ Feature Engineering
New meaningful features were created:
- **FamilySize** = `SibSp + Parch + 1`
- **IsAlone** → identifies solo travelers
- **Title** → extracted from passenger names (Mr, Mrs, Miss, Master, etc.)

These features significantly improved interpretability of survival patterns.

---

## 🔥 Correlation Analysis
- Identified correlations between numerical features
- Found strong relationships between survival and:
  - Passenger class
  - Fare
  - Cabin availability
  - Family-related features

---

## 📄 Automated Data Profiling
- Generated a **ydata-profiling report**
- Provided automatic insights on:
  - Missing values
  - Feature distributions
  - Correlations
  - Data quality warnings

📁 The profiling report is available as an **HTML file** for easy viewing.

---

## 🛠️ Tools & Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- ydata-profiling
- Google Colab
- VS Code
- Git & GitHub

---

## ✅ Key Insights
- Females and children had significantly higher survival rates
- 1st class passengers survived more than others
- Passengers with cabins and higher fares had better chances of survival
- Small families survived better than solo travelers
- Titles like `Mrs`, `Miss`, and `Master` were strong survival indicators

---

## 🚀 Outcome
This project builds a strong foundation for:
- Feature selection
- Data preprocessing
- Machine learning model development

It also demonstrates a **real-world data analysis workflow**.

---

## 📌 Next Steps
- Apply machine learning models to predict survival
- Experiment with feature scaling and encoding
- Evaluate model performance

---

## 🏆 Part of
**21 Days – 21 Machine Learning Projects Challenge**

📅 **Day 01 Completed Successfully ✅**
