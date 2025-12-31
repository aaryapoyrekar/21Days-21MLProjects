# 🗣️ Talk to Your Data  
## Project 15: Text-to-SQL via Prompt Engineering

---

## 📌 Project Overview

This project implements a **Natural Language to SQL (Text-to-SQL)** system that enables users to query an **e-commerce database** using plain English. Instead of writing SQL manually, users can ask analytical and business questions in natural language and receive accurate results directly from the database.

The system uses **Google Gemini** along with **prompt engineering** to translate user intent into valid **SQLite SQL queries**, execute them on a real database, and return the results in a structured tabular format.

---

## 🎯 Project Goals

- Enable conversational querying of structured e-commerce data  
- Convert natural language questions into executable SQL queries  
- Support joins, filtering, aggregation, ranking, and sorting  
- Execute AI-generated SQL on a real SQLite database  
- Demonstrate a complete end-to-end Text-to-SQL pipeline  

---

## ⚙️ How the System Works

User Question (English)
        ↓
Prompt Engine (Schema + Rules)
        ↓
Gemini AI (Text-to-SQL)
        ↓
Generated SQLite SQL
        ↓
SQLite Database Execution
        ↓
Results as Pandas DataFrame


---

## 🧠 Prompt Engineering Strategy

The prompt is designed using a structured framework:
- **Role**: Expert Text-to-SQL translator  
- **Context**: Database schema and relationships  
- **Task**: Generate accurate SQL queries  
- **Constraints**: SQLite syntax, no hallucinated columns, no table modification  
- **Examples**: Few-shot prompting for consistency  

This ensures reliable and executable SQL generation.

---

## 🔍 Example Natural Language Queries

- What are my most popular products?
- Show me the order count by country.
- Which country ranks in the middle by total sales?
- What is the 2nd highest sold product for each country?
- On which day of the week do I get the most orders?

---

## 🧪 Technologies Used

- Python  
- SQLite  
- Pandas  
- Google Gemini API  
- Prompt Engineering  
- Mockaroo (synthetic data generation)

---

## 🚀 Key Learnings

- Translating human intent into structured SQL queries  
- Importance of schema grounding to reduce hallucinations  
- Designing effective prompts for analytical SQL generation  
- Building real AI systems on top of relational databases  

---

## 📈 Future Enhancements

- Add query validation and safety checks  
- Integrate Retrieval-Augmented Generation (RAG)  
- Support more complex analytical queries  
- Build a conversational user interface  

