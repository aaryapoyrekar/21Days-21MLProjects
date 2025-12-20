# 📈 Project 6: Time Series Analysis & Forecasting 

## 📌 Project Overview
This project focuses on **time series analysis and forecasting** using the classic **Airline Passengers dataset**.  
The goal is to understand time-dependent data, make it stationary, and build forecasting models using **ARIMA** and **SARIMA**.

The project follows a **step-by-step, real-world workflow** — from exploratory analysis and stationarity testing to model building, evaluation, and comparison with smoothing techniques.

---

## 🎯 Project Objective
To build a robust time series model that can **accurately forecast future airline passenger counts**, while demonstrating:
- Why stationarity is required
- How ARIMA and SARIMA models work
- Why SARIMA is better for seasonal data

---

## 📂 Dataset
- **Dataset:** Monthly Airline Passenger Data (1949–1960)
- **Frequency:** Monthly
- **Records:** 144 observations
- **Target Variable:** `Passengers`

---

## 🧠 Core Concepts Covered

1. **Time Series Fundamentals**
   - Trend
   - Seasonality
   - Residuals (Noise)

2. **Stationarity**
   - What stationarity means
   - Why ARIMA requires stationary data
   - Augmented Dickey-Fuller (ADF) Test

3. **Data Transformation**
   - Log transformation to stabilize variance
   - Differencing to remove trend

4. **Model Identification**
   - ACF (Autocorrelation Function)
   - PACF (Partial Autocorrelation Function)

5. **ARIMA Modeling**
   - Building ARIMA(1,1,1)
   - Understanding its limitations for seasonal data

6. **SARIMA Modeling**
   - Extending ARIMA to handle seasonality
   - SARIMA(1,1,1)(1,1,1,12)

7. **Forecasting & Evaluation**
   - Forecast visualization
   - RMSE-based evaluation
   - Model comparison

---

## 🔍 Workflow Summary

### 1️⃣ Exploratory Data Analysis (EDA)
- Visualized passenger trends
- Identified:
  - Upward trend
  - Strong yearly seasonality
  - Increasing variance

### 2️⃣ Time Series Decomposition
- Decomposed data into:
  - Trend
  - Seasonal
  - Residual components

### 3️⃣ Stationarity Testing
- Applied **ADF test**
- Original data:
  - ❌ Non-stationary (p-value ≈ 0.99)

### 4️⃣ Making the Series Stationary
- Applied:
  - Log transformation
  - First-order differencing
- Re-tested using ADF:
  - ✅ Stationary (p-value < 0.05)

### 5️⃣ Model Identification
- **PACF → p = 1**
- **ACF → q = 1**
- Selected model: **ARIMA(1,1,1)**

### 6️⃣ ARIMA Model
- Captured overall trend
- ❌ Failed to capture seasonality

### 7️⃣ SARIMA Model
- Model: **SARIMA(1,1,1)(1,1,1,12)**
- Successfully captured:
  - Trend
  - Annual seasonality
- Provided superior forecasts

### 8️⃣ Final Evaluation
- Compared actual vs forecasted values
- Calculated **RMSE**
- SARIMA showed **lower error and better alignment**

---

## 📊 Model Comparison Summary

| Model | Trend | Seasonality | Forecast Accuracy |
|------|------|-------------|------------------|
| Moving Average | ✅ | ❌ | Low |
| Exponential Smoothing | ✅ | ❌ | Medium |
| ARIMA | ✅ | ❌ | Medium |
| **SARIMA** | ✅ | ✅ | **High** |

---

## ✅ Final Conclusion
- The original airline passenger data was **non-stationary**
- After transformation, stationarity was achieved (**p-value < 0.05**)
- ARIMA served as a good baseline model
- **SARIMA outperformed all other methods** by capturing both trend and seasonality
- SARIMA is the most suitable model for **seasonal time series data**

---

## 🛠️ Tools & Libraries Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Statsmodels
- Scikit-learn

---


## 🚀 Next Steps
- Hyperparameter tuning with grid search
- Forecasting future unseen months
- Deploying forecasts in a dashboard
