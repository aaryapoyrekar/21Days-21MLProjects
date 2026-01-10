# 🤖 Building an AI-Powered Pipeline with n8n

This repository documents my learning and implementation of an **AI-powered automation pipeline using n8n**, completed as **Day 21** of the *21 Days – 21 AI Projects* challenge.

---

## 🔍 What is n8n?

**n8n** (pronounced *n-eight-n* or *nodemation*) is a powerful, low-code workflow automation platform that allows users to connect applications, APIs, and services to automate tasks and build complex pipelines with minimal coding.

It uses a **node-based visual editor**, where workflows are created by connecting nodes that represent actions, triggers, or transformations.

Key characteristics:
- Low-code / no-code
- Source-available
- Self-hostable
- Highly extensible
- Ideal for AI-powered automation workflows

---

## ⚙️ Core Automation Concepts

### 1️⃣ Automation
Automation is a predictable sequence of predefined actions that transfer data from one system to another with minimal human intervention.

---

### 2️⃣ Trigger
A trigger initiates a workflow.

**Types of triggers:**
- Manual (button click)
- Scheduled (every X hours/days)
- Event-based (form submission, Git push, webhook, etc.)

---

### 3️⃣ Filters & Conditionals
Filters control the flow of data based on conditions.

Examples:
- If gender = male → do X
- If customer = HNI → do Y
- Sorting, formatting, transforming data

---

### 4️⃣ Actions
Actions perform tasks using third-party tools or internal logic.

Examples:
- Update a database record
- Send an email or Slack message
- Upload a file to cloud storage
- Call an external API
- Generate AI-based content

---

## 🧱 Nodes in n8n

Nodes are the **building blocks (atoms)** of n8n workflows.

### Categories of Nodes:
1. **Entry Nodes** – Triggers
2. **Function Nodes** – Filters, transformations, logic
3. **Exit Nodes** – Persistence, notifications, storage

### Node Types:
- Triggers
- App Actions
- Data Transformation
- Flow Control
- Files
- Advanced / AI nodes

---

## 🧠 AI-Powered Workflows with n8n

n8n can integrate AI models into workflows to:
- Summarize text
- Generate content
- Classify data
- Build AI agents
- Automate decision-making pipelines

This project demonstrates how AI can be embedded directly into automation pipelines.

---

## 📌 Sample Workflow Implemented

### 📰 Newspaper AI Agent
An AI-powered workflow that:
1. Fetches live news via an API
2. Structures the news data
3. Sends it to an AI Agent
4. Generates a clean, formal newspaper-style article

---

## 🖥️ Run n8n Locally (Docker)

```bash
docker volume create n8n_data

docker run -it --rm \
  --name n8n \
  -p 5678:5678 \
  -v n8n_data:/home/node/.n8n \
  docker.n8n.io/n8nio/n8n

## 🚀 Accessing n8n Editor

Access the n8n editor locally at:  
👉 http://localhost:5678

---

## 🧪 Practice Workflows (Hands-On)

Try building and sharing screenshots for the following workflows:

- **Your First AI Agent**
- **AI Newsletter Automation v0.1**
- **AI Newsletter Automation v1.0**
- **API-based Data Pipelines**
- **Content Summarization Workflows**

Explore more community workflows here:  
👉 https://n8n.io/workflows/

---

## 🛠 Tech Stack Used

- **n8n** – Workflow automation
- **Docker** – Local deployment
- **NewsAPI** – News data source
- **Google Gemini** – AI content generation
- **JSON** – Workflow definitions

---

## 📚 Learning Outcomes

- Understanding workflow automation concepts
- Designing node-based automation pipelines
- Integrating external APIs into workflows
- Building AI agents inside automation tools
- Prompt engineering for structured outputs
- Debugging and scaling workflows
- Developing real-world automation thinking

---

## 🏁 Project Context

This project marks the **final day (Day 21)** of the  
**21 Days – 21 AI Projects** challenge.

Special thanks to **GeeksforGeeks** for structured learning guidance and inspiration throughout the journey.
