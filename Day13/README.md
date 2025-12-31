# 📈 Stock Price Prediction using Machine Learning & Deep Learning (NIFTY 50)

## 🔍 Project Overview
This project explores **time-series stock price prediction** using a combination of **traditional Machine Learning models** and **Deep Learning sequence models** on the **NIFTY 50 index**.

Instead of relying on a single algorithm, the project builds a **flexible and extensible pipeline** that:
- Converts raw historical prices into supervised learning data
- Trains multiple models on different time windows
- Evaluates performance using robust error metrics
- Compares classical ML approaches with neural network–based models

The primary goal is to understand **how model choice and input window size affect predictive performance** on real-world financial data.

---

## 📂 Dataset
- **Source:** Kaggle – NIFTY 50 (25 Years Data)
- **Link:** https://www.kaggle.com/datasets/ashishjangra27/nifty-50-25-yrs-data

### Features Used
- Open  
- High  
- Low  
- Close  

The project focuses on **univariate time-series forecasting**, where past values of a single price feature are used to predict the next value.

---

## 🔁 Project Pipeline

### 1️⃣ Data Preparation
- Historical stock prices are loaded from CSV
- Time-series data is transformed into supervised learning format using a **sliding window technique**
- Input windows represent past *N* days, and the target is the next day’s price

### 2️⃣ Feature Engineering
- Sliding windows of multiple lengths (e.g., 30, 60, 90 days)
- Enables analysis of short-term vs long-term dependencies

---

## 🤖 Models Implemented

### 🔹 Machine Learning Models
- K-Nearest Neighbors (KNN)
- Linear Regression (baseline exploration)
- Other regressors explored during experimentation

### 🔹 Deep Learning Models
- Simple RNN
- GRU (Gated Recurrent Unit)
- LSTM (Long Short-Term Memory)
- Bidirectional LSTM  

All deep learning models are implemented using **TensorFlow / Keras Sequential API** and trained on sequential inputs.

---

## ⚙️ Training Strategy
- Train–test split: **90% training / 10% testing**
- Deep learning models trained for multiple epochs to capture temporal patterns
- Early stopping used to prevent overfitting and reduce training time
- Models are trained independently for different input window sizes

---

## 📊 Evaluation Metrics
Model performance is evaluated using:
- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**

Both training and testing metrics are tracked to analyze:
- Overfitting vs generalization
- Stability across time windows
- Relative performance of ML vs DL models

---

## 📈 Analysis & Insights
The project includes:
- Comparison of models across different time horizons
- Identification of price types that are more predictable
- Visualization of model performance using plots and tables

Key insights observed:
- Longer time windows help sequence models capture temporal dependencies
- Deep learning models outperform traditional ML models for longer sequences
- Simpler models like KNN remain competitive for shorter windows

---

## 💾 Model Persistence & Reproducibility
- Evaluation results are saved as CSV for reuse
- Models can be reloaded for inference
- The pipeline is designed to be modular and easily extensible

---

## 🛠️ Tech Stack
- **Python**
- **NumPy, Pandas**
- **Scikit-learn**
- **TensorFlow / Keras**
- **Matplotlib**
- **Joblib**
- **Google Colab**

---

## 🎯 Learning Outcomes
Through this project, I gained hands-on experience with:
- Time-series data transformation
- Sliding window forecasting
- ML vs DL trade-offs
- Handling long-running experiments in Colab
- Model evaluation beyond accuracy metrics
- Practical challenges of real-world financial data

---

## 🚀 Future Improvements
- Multivariate time-series modeling
- Hyperparameter tuning
- Incorporating technical indicators
- Walk-forward validation
- Deployment as a web application or API

---

## 📌 Project Status
✅ Completed core pipeline  
📊 Results analyzed and visualized  
📁 Ready for extension and optimization  

---

