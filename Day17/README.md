# 📸 Day 17 – Multimodal RAG: Semantic Image Search using Gemini & Chroma

This project demonstrates a **Multimodal Retrieval-Augmented Generation (RAG)** pipeline that enables **semantic search over images** using natural language queries.  
Images are first converted into rich textual metadata using **Gemini Vision**, embedded using **Google’s embedding model**, and stored in a **Chroma vector database** for efficient retrieval.

This project was built as **Day 17** of the **21 Days – 21 ML Projects** challenge.

---

## 🚀 Project Overview

Traditional image search relies on filenames or tags.  
This project goes beyond that by enabling **conceptual and semantic image search**, such as:

- “a classroom workshop”
- “student studying with a laptop”
- “coding workspace at night”

### Key Idea:
> Convert images → structured text → vector embeddings → semantic search

---

## 🧠 What This Project Does

1. Takes a **personal synthetic image dataset** (academic & workspace images)
2. Uses **Gemini Vision** to generate structured metadata:
   - Main subject
   - Detailed scene description
   - Visual elements
   - Visible text (if any)
   - Search-optimized keywords
3. Stores metadata as JSON
4. Converts metadata into **vector embeddings**
5. Saves embeddings in a **Chroma vector database**
6. Retrieves relevant images using **natural language queries**

---

## 🗂️ Dataset

- **Type:** Synthetic personal dataset
- **Images:** 16 AI-generated images
- **Theme:**  
  - Classrooms  
  - Workshops  
  - Coding environments  
  - Study desks  
  - Presentations  

Images were generated using **generative AI** to simulate personal academic environments.

---

## 🏗️ Project Architecture

Images
↓
Gemini Vision (Metadata Generation)
↓
Structured JSON
↓
Text Embeddings (text-embedding-004)
↓
Chroma Vector Database
↓
Semantic Search Queries
↓
Relevant Images Retrieved


---

## 🛠️ Tech Stack

- **LLM / Vision Model:** Google Gemini 2.5 Flash
- **Embeddings:** Google `text-embedding-004`
- **Vector Database:** Chroma
- **Framework:** LangChain
- **Environment:** Google Colab
- **Language:** Python

---

## 📂 Project Structure

Day17_RAG/
│
├── img_01.jpg
├── img_02.jpg
├── ...
├── img_16.jpg
│
├── jsons/
│ ├── img_01.json
│ ├── img_02.json
│ └── ...
│
├── chroma_db/
│ └── (persisted vector data)
│
└── notebook.ipynb


---

## 🔍 Example Queries

```python
search_images("classroom workshop")
search_images("student studying with laptop")
search_images("coding workspace")
search_images("presentation slide")
```

## ✨ Key Learnings

- Prompt engineering is critical for structured vision outputs  
- Multimodal RAG enables powerful cross-modal retrieval  
- Vector databases are essential for scalable semantic search  
- Domain-specific datasets improve retrieval quality  
- Synthetic data is effective for experimentation and learning  

---

## 📌 Why This Matters

This approach is highly relevant for:

- Digital asset management systems  
- Enterprise search  
- Knowledge bases  
- Media libraries  
- AI-powered content discovery  

It demonstrates how **LLMs + Vision + Vector Databases** can work together in real-world systems.

---

## 📅 Project Context

- **Series:** 21 Days – 21 ML Projects  
- **Day:** 17  
- **Focus:** Multimodal RAG & Semantic Image Retrieval  

---

## 🙌 Acknowledgements

- Google Gemini & AI Studio  
- LangChain  
- ChromaDB  
- Google Colab  
