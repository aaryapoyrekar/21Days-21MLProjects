# 🛍️ Customer Segmentation with Clustering

## 📌 Project Overview
This project focuses on **customer segmentation** using **unsupervised machine learning** techniques.  
The goal is to identify meaningful customer groups based on **age, income, and spending behavior**, and convert these patterns into **actionable business insights**.

Customer segmentation helps businesses understand different types of customers and design **targeted marketing strategies**, loyalty programs, and personalized offers.

---

## 🎯 Objectives
- Understand customer behavior using exploratory data analysis (EDA)
- Apply clustering techniques to discover hidden patterns
- Compare multiple clustering approaches
- Create interpretable customer personas from clusters

---

## 🧠 Key Concepts Used
- Unsupervised Learning
- K-Means Clustering
- Elbow Method (WCSS)
- Feature Scaling
- Feature Engineering
- Hierarchical Clustering
- Customer Persona Analysis

---

## 📊 Dataset Description
The dataset contains mall customer information with the following features:
- **Gender**
- **Age**
- **Annual Income (k$)**
- **Spending Score (1–100)**

The `CustomerID` column was removed as it does not contribute to clustering.

---

## 🔍 Exploratory Data Analysis (EDA)
- Studied individual feature distributions (age, income, spending)
- Analyzed relationships using pair plots and 3D visualization
- Identified **Annual Income vs Spending Score** as the strongest clustering dimension
- Observed that gender does not strongly influence spending behavior

---

## 🤖 Clustering Models Built

### 1️⃣ Income & Spending Score Clustering
- Used **K-Means** with optimal `k` selected via the **Elbow Method**
- Identified clear customer segments such as:
  - High income–high spending customers
  - High income–low spending customers
  - Budget shoppers
  - Enthusiastic spenders

---

### 2️⃣ Age & Spending Score Clustering
- Built an alternative segmentation model
- Revealed age-based spending patterns:
  - Young high spenders
  - Young low spenders
  - Older moderate spenders
  - Older low spenders

---

## 🛠️ Feature Engineering
A new feature, **Spending Power Index**, was created by combining:
- Annual Income
- Spending Score

This engineered feature produced **cleaner and more interpretable clusters**, highlighting:
- Premium customers
- Impulsive young buyers
- Cautious older spenders

---

## 🌳 Hierarchical Clustering
- Applied hierarchical clustering as an alternative method
- Used a **dendrogram** to visualize cluster formation
- Confirmed the optimal number of clusters found using K-Means

---

## 📈 Key Insights
- Income alone does not define spending behavior
- Combining features improves clustering quality
- Feature engineering enhances business interpretation
- Different clustering views reveal different customer perspectives

---

## 🧾 Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Plotly
- Scikit-learn
- SciPy

---

## 🚀 Conclusion
This project demonstrates how **unsupervised learning** can uncover valuable customer segments without labeled data.  
By combining EDA, clustering, and feature engineering, the analysis delivers **practical insights** that businesses can directly act upon.

---

📂 Part of **21 Days – 21 Machine Learning Projects**
