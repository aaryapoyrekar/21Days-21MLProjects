# 📅 Day 11 – Hugging Face Pipelines & Diffusion Models

## 📌 Project Overview
This project explores the **Hugging Face ecosystem** and demonstrates how powerful **pre-trained, open-source models** can be used through simple **pipelines** to solve a wide range of AI tasks.

The notebook first showcases multiple **NLP and Computer Vision pipelines** provided by Hugging Face, and then dives deeper into **image generation using diffusion models** as part of the assignment.

The goal of this project is to understand **how modern AI capabilities can be accessed easily without training models from scratch**, using community-driven open-source tools.

---

## 🤗 About Hugging Face
**Hugging Face** is a leading open-source AI platform that provides:
- Pre-trained models
- Ready-to-use pipelines
- Datasets and demos
- Tools for both research and production

Its ecosystem enables developers to apply state-of-the-art AI models with **just a few lines of code**.

---

## 🔧 Pipelines Covered
The notebook demonstrates the following Hugging Face pipelines:

### 🔹 Natural Language Processing (NLP)
- **Sentiment Analysis** – Classifying text sentiment
- **Text Summarization** – Generating concise summaries
- **Question Answering** – Extracting answers from context
- **Named Entity Recognition (NER)** – Identifying entities in text
- **Text Generation** – Generating text from prompts
- **Translation** – Translating text between languages
- **Zero-Shot Classification** – Classifying text without task-specific training

### 🔹 Computer Vision
- **Image Classification** – Assigning labels to images
- **Object Detection** – Detecting and localizing objects
- **Image Segmentation** – Pixel-level object segmentation
- **Image Captioning** – Generating text descriptions for images

Each task is implemented using **pre-trained open-source models** available on the Hugging Face Hub.

---

## 🎨 Assignment: Image Generation with Diffusion Models

### 🔹 Objective
To explore **text-to-image generation** using diffusion-based models from Hugging Face.

### 🔹 Model Used
- **`runwayml/stable-diffusion-v1-5`**
- Loaded using **Hugging Face Diffusers Pipeline**

### 🔹 Key Concepts
- Diffusion-based image generation
- Prompt engineering
- Inference steps and guidance scale
- GPU acceleration for faster generation

### 🔹 What Was Done
- Loaded a Stable Diffusion pipeline
- Generated multiple images using different prompts
- Visualized generated images using Matplotlib
- Analyzed the impact of prompts and parameters on image quality

---

## 🧠 Learnings & Takeaways
- Hugging Face pipelines abstract complex AI workflows into simple APIs
- Open-source models enable rapid experimentation and innovation
- Diffusion models are highly effective for creative image generation
- Prompt quality plays a critical role in generative AI outputs
- Modern AI applications can be built without training models from scratch

---

## 🛠️ Tech Stack & Tools
- **Python**
- **Hugging Face Transformers**
- **Hugging Face Diffusers**
- **PyTorch**
- **Matplotlib**
- **PIL**


---

## 🚀 Conclusion
This project highlights the power of **open-source AI and Hugging Face pipelines** in building real-world NLP, Computer Vision, and Generative AI applications with minimal effort.  
Day 11 serves as a strong foundation for understanding how modern AI systems are built and deployed using community-driven tools.

---

📌 *Part of the **21 Days – 21 Machine Learning Projects** learning journey.*
