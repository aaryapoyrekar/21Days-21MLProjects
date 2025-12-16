# 🎬 Day 02 – Netflix Content Analysis (Exploratory Data Analysis)

## 📌 Project Overview
This project performs an in-depth Exploratory Data Analysis (EDA) on the Netflix dataset to understand content trends, production strategies, audience targeting, and platform growth over time.

Instead of applying machine learning models, this project focuses on understanding the data through cleaning, visualization, feature engineering, and basic text analysis.

---

## 🎯 Objective
- Analyze Netflix’s content library using EDA techniques  
- Compare Movies vs TV Shows distribution  
- Study content ratings and audience focus  
- Analyze trends based on release year vs year added  
- Understand content age and acquisition strategy  

---

## 🧠 What is Exploratory Data Analysis (EDA)?
Exploratory Data Analysis is the process of:
- Understanding the structure of the dataset  
- Identifying missing values and data quality issues  
- Studying feature distributions and trends  
- Discovering relationships between variables  

EDA helps draw meaningful insights before applying machine learning or advanced analytics.

---

## 🗂️ Dataset Information
- **Dataset Name:** Netflix Titles Dataset  
- **Total Records:** ~7,800 titles  
- **Content Types:** Movies and TV Shows  

### 🔑 Key Features
- Type (Movie / TV Show)  
- Release Year  
- Date Added  
- Rating  
- Duration  
- Genre (`listed_in`)  
- Country  
- Director and Cast  
- Description  

---

## 🧹 Data Cleaning & Preprocessing
The following steps were performed:
- Filled missing values in **director** and **cast** with `"Unknown"`  
- Filled missing **country** values using the most frequent country  
- Removed rows with missing **date_added** and **rating**  
- Converted `date_added` from string to datetime format  
- Extracted **year_added** and **month_added**  
- Created a new feature: **content_age = year_added − release_year**

---

## 📊 Exploratory Data Analysis Performed

### 🔹 Content Distribution Analysis
- Compared Movies vs TV Shows  
- Found Netflix’s catalog to be movie-dominant  

### 🔹 Time-Series Analysis
- Analyzed yearly content additions  
- Observed rapid growth between 2016–2019  
- Noted slowdown in recent years (COVID impact / incomplete data)  

### 🔹 Ratings Analysis
- Studied content ratings over time  
- Identified dominance of mature ratings like **TV-MA** and **TV-14**

### 🔹 Genre Analysis
- Processed multi-valued genre data  
- Found **International Movies, Dramas, and Comedies** as top genres  

### 🔹 Content Duration Analysis
- Movies mostly fall in the **80–120 minute** range  
- Most TV shows have **only one season**

### 🔹 Geographical Analysis
- Identified top content-producing countries  
- United States leads, followed strongly by India  

---

## 🛠️ Feature Engineering
New features created:
- **Year Added**  
- **Month Added**  
- **Content Age**

These features helped distinguish Netflix Originals from licensed content.

---

## 📝 Text Analysis
- Analyzed content descriptions using word frequency and word-pair analysis  
- Identified recurring themes related to life, relationships, youth, and personal journeys  

---

## 🎬 Director Analysis
- Identified most frequent directors on Netflix  
- Observed significant missing director metadata (`Unknown`)  
- Among known directors, repeated collaborations were visible

---

## 📈 Key Insights
- Netflix focuses heavily on movies over TV shows  
- Majority of content targets mature audiences  
- Movies tend to be older; TV shows are newer  
- Netflix increasingly adds content closer to release year  
- Strong emphasis on international content  

---

## 🛠️ Tools & Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Jupyter Notebook  
- VS Code  
- Git & GitHub  

---

## 🚀 Outcome
This project demonstrates a complete EDA workflow and provides strong insights into Netflix’s content strategy. It builds a solid foundation for future analytics and machine learning projects.

---

## 🏆 Part of
**21 Days – 21 Projects (Data Science / ML / AI Challenge)**  

📅 **Day 02 Completed Successfully ✅**
