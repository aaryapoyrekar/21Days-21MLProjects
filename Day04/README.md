# 🩺 Heart Disease Prediction using Machine Learning

## 📌 Project Overview
Heart disease is one of the leading causes of mortality worldwide. Early detection plays a crucial role in reducing risks and improving patient outcomes.

This project focuses on building a **machine learning–based classification system** to predict the presence and severity of heart disease using clinical and medical attributes. The project follows a complete machine learning workflow — from data understanding and preprocessing to model training and evaluation.

---

## 🎯 Objectives
- Analyze medical factors associated with heart disease
- Perform detailed **Exploratory Data Analysis (EDA)** to uncover patterns
- Preprocess real-world healthcare data effectively
- Train a classification model to predict heart disease
- Interpret results in a medical and practical context

---

## 📂 Dataset
- **Source:** UCI Heart Disease Dataset (via Kaggle)
- **Type:** Structured medical data
- **Target Variable (`num`):**
  - `0` → No heart disease  
  - `1–4` → Presence and increasing severity of heart disease  

### Key Features
- `age` – Age of the patient  
- `sex` – Gender  
- `cp` – Chest pain type  
- `trestbps` – Resting blood pressure  
- `chol` – Serum cholesterol  
- `thalch` – Maximum heart rate achieved  
- `exang` – Exercise-induced angina  
- `oldpeak` – ST depression  
- `ca` – Number of major vessels  
- `thal` – Thalassemia type  

---

## 🔍 Exploratory Data Analysis (EDA)
EDA was conducted to understand the structure and behavior of the data, including:

- Distribution of heart disease severity
- Relationship between age and disease occurrence
- Impact of exercise capacity (max heart rate) on heart disease
- Chest pain types and their association with disease
- Presence of outliers in blood pressure and cholesterol
- Correlations among medical attributes

### Key Insights
- Lower maximum heart rate is strongly associated with heart disease
- Asymptomatic chest pain is a strong indicator of disease
- Age increases risk but is not sufficient alone
- Accurate prediction requires **multivariate analysis**

---

## 🔗 Machine Learning Pipeline (Conceptual Overview)

Although preprocessing and model training in this project are implemented **manually** for learning clarity, the overall workflow follows a **standard machine learning pipeline**, which is an industry best practice.

### Pipeline Stages Followed
1. **Data Ingestion**  
   - Load and inspect raw medical data.

2. **Exploratory Data Analysis (EDA)**  
   - Identify distributions, correlations, outliers, and feature–target relationships.

3. **Data Preprocessing**  
   - Handle missing numerical and categorical values  
   - Encode categorical features using one-hot encoding  
   - Scale numerical features for uniform contribution  

4. **Model Training**  
   - Train a classification model to predict heart disease.

5. **Model Evaluation**  
   - Assess performance using precision, recall, F1-score, and confusion matrix.

### Why Pipelines Matter
In real-world ML systems, pipelines:
- Prevent data leakage
- Ensure consistent preprocessing during training and inference
- Improve reproducibility and maintainability

Manual preprocessing in this project helps demonstrate a **clear understanding of each pipeline stage**.

---

## 🧹 Data Preprocessing
The following preprocessing steps were applied:
- Missing numerical values filled using mean
- Missing categorical values filled using mode
- Categorical features encoded using **One-Hot Encoding**
- Numerical features standardized using **StandardScaler**

---

## 🤖 Model Building
A **Logistic Regression** classifier was used for prediction.

### Why Logistic Regression?
- Simple and interpretable
- Well-suited for medical classification problems
- Provides probabilistic outputs useful for healthcare decision-making

---

## 📊 Model Evaluation
The model was evaluated using:
- **Precision**
- **Recall**
- **F1-Score**
- **Confusion Matrix**

Special emphasis was placed on **recall**, as false negatives in medical diagnosis can have serious consequences.

---

## 🧠 Key Learnings
- Medical data requires careful preprocessing and analysis
- EDA directly influences preprocessing and model choice
- Interpretability is crucial in healthcare-related ML models
- Machine learning can assist clinicians but not replace them

---

## 🚀 Future Improvements
- Convert the task into binary classification (disease vs no disease)
- Address class imbalance using resampling techniques
- Experiment with ensemble models (Random Forest, XGBoost)
- Perform hyperparameter tuning
- Deploy the model as a web application

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---


