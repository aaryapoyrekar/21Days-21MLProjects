# 📘 Day 14 – Build Your Own GPT: Tiny LLM Story Generator

This project demonstrates how to **build, train, and evaluate a small GPT-2–style language model from scratch** to generate short children’s stories using the **TinyStories dataset**.  
It walks through the **complete lifecycle of a language model** — from data streaming and tokenization to custom training loops, checkpointing, and inference.

> 🚀 Part of the **21 Days – 21 ML / GenAI Projects** learning journey.

---

## 🔍 Project Overview

Large Language Models (LLMs) are powerful but expensive to train. This project focuses on **Tiny LLMs** — compact transformer models that can be trained efficiently on limited resources (e.g., Google Colab) while still demonstrating core LLM concepts.

The model is trained to generate **simple, coherent short stories** suitable for children, using a curated dataset designed specifically for small language models.

---

## 🎯 Objectives

- Understand how GPT-style causal language models work
- Train a **custom GPT-2–like model from scratch**
- Learn how **next-token prediction** is implemented
- Build a **custom PyTorch training loop**
- Handle **streaming datasets** efficiently
- Save and reload model checkpoints
- Perform qualitative evaluation through text generation

---

## 📚 Dataset

**TinyStories**  
- Source: Hugging Face Datasets (`roneneldan/TinyStories`)
- Description: A large collection of short, simple stories designed for training and evaluating small language models
- Loaded in **streaming mode** to avoid memory issues

Why TinyStories?
- Simple vocabulary and sentence structure
- Ideal for fast experimentation
- Perfect for understanding LLM training fundamentals

---

## 🧠 Model Architecture

A compact GPT-2–style transformer:

- Vocabulary size: GPT-2 tokenizer vocabulary
- Context length: 512 tokens
- Embedding size: 256
- Transformer layers: 4
- Attention heads: 4
- Objective: **Causal Language Modeling (next-token prediction)**

This architecture balances **learning capacity** and **training efficiency**.

---

## 🛠️ Key Components

### 1️⃣ Data Pipeline
- Streaming dataset (`IterableDataset`)
- Text cleaning and normalization
- Tokenization using GPT-2 tokenizer
- Dynamic padding via custom `collate_fn`

### 2️⃣ Training Loop
- Custom PyTorch training loop
- AdamW optimizer
- Gradient clipping for stability
- Gradient accumulation for memory efficiency
- Mixed precision (FP16) for faster training
- Periodic checkpoint saving

### 3️⃣ Checkpointing
- Model and tokenizer saved after each epoch
- Training history stored as JSON
- Resume training supported from any saved checkpoint

### 4️⃣ Inference & Evaluation
- Generate short story continuations from prompts
- Compare outputs with a pretrained TinyStories model
- Qualitative evaluation of coherence and creativity

---

## 🧪 Sample Prompts

- “Once upon a time”
- “Once there was a little boy”
- “Once there was a cute little animal”

The generated outputs improve gradually as training progresses.

---

## ⚙️ Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Google Colab (GPU)
- TQDM for progress tracking

---

## 📈 Learnings & Takeaways

- Training LLMs is **data- and memory-intensive**
- Streaming datasets are essential for large corpora
- Dynamic padding significantly reduces memory usage
- Checkpointing is critical when working on unstable runtimes
- Even small models can generate meaningful text with proper training

---

## 🚧 Limitations

- Model is trained on a limited subset of data per epoch (resource constraints)
- Outputs may lack long-range coherence
- Designed for learning and experimentation, not production use

---

## 🔮 Future Improvements

- Train for more epochs or larger subsets
- Experiment with larger embedding sizes or deeper models
- Add perplexity-based evaluation
- Fine-tune on specific storytelling styles
- Deploy as a lightweight web demo

---

## 🙌 Acknowledgements

- **TinyStories Dataset** by Ronen Eldan
- **Hugging Face** for Transformers & Datasets
- **GeeksforGeeks** – “21 Projects, 21 Days: ML, DL & GenAI” course
- Instructor & mentors for structured guidance

---

## 📌 Project Tag

**Day 14 – Build Your Own GPT (Tiny LLM Story Generator)**  
Part of *21 Days | 21 Projects*

---

Happy Learning & Happy Coding 🚀

