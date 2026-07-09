<div align="center">

# Hi, I'm Pragy Upadhyay 👋

**Data Analyst · Machine Learning Engineer · Full-Stack AI Developer**

*Final-year ECE student at JIIT Noida — building production-ready AI systems, not just models.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/pragy-upadhyay-893895246)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/pragy34)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:pragy34@gmail.com)

</div>

---

## 🚀 What Makes Me Different

* I build **end-to-end AI systems** — not just models
* I ship **production-ready applications**, not just notebooks
* I combine **ML + Backend + UI** into complete products
* I focus on **explainability, reasoning, and real-world usability**

👉 Most candidates show models. I show **systems that actually work in real life.**

---

## 🧭 What I Build

I design and deploy **complete AI products** — from raw data to real users.

* 🤖 Machine Learning & Deep Learning (ML → LSTM → SNN)
* ⚙️ Full-Stack AI Apps (FastAPI/Express + React/Next.js + PostgreSQL)
* 🧠 Generative AI & LLM Systems (reasoning + prompt pipelines + structured outputs)
* 🔊 Event-Driven & Resilient Data Pipelines
* 📊 Data Analytics & Visualization Systems

---

## 🏆 Featured Projects

### 📥 csv2crm — AI-Powered CRM CSV Importer

🔗 Live demo: https://csv2crm.vercel.app
🔗 Backend API: https://csv2crm.onrender.com
🔗 Repo: https://github.com/pragy34/csv2crm

> Upload *any* leads/CRM CSV — Facebook Ads exports, Google Ads exports, custom spreadsheets, any layout — and an LLM intelligently maps it into a fixed CRM schema.

* Client-side parse-and-preview (no AI cost until the user confirms) using **papaparse**, then batched AI extraction on the backend
* AI provider abstracted behind a common interface — runs on **Groq** in production for fast inference and **strict JSON Schema structured outputs**, with **Gemini** as a swappable fallback
* Prompt and response schema both generated from a **single source-of-truth CRM schema** (`crmSchema.ts`), so the prompt, the JSON schema sent to the model, and the `zod` server-side validator can never drift out of sync
* Batches processed with a concurrency cap + exponential-backoff retries; a failed batch degrades to "skipped with reason" instead of failing the whole import
* Real-time import progress via **Server-Sent Events**, not a simulated timer

💡 Demonstrates **AI prompt engineering discipline + backend resilience design**, not just "call an LLM and hope"

**Tech:** Next.js 14, TypeScript, Tailwind, Express, zod, Groq, Google Gemini

---

### 🎙️ Audio Transcription Pipeline — Resilient Event-Driven Whisper System

🔗 Repo: https://github.com/pragy34/audio-transcription-pipeline

> A production-minded audio transcription pipeline built around OpenAI Whisper — designed after seeing a naive "just call Whisper on upload" approach fail silently on real-world audio.

* **Format detection by file bytes** (via `libmagic`), not by trusting the file extension — because users rename files and uploads get mislabeled
* **Validation gate** rejects unsupported formats, zero-byte files, corrupt/undecodable audio, oversized files, and silent/too-short clips *before* they hit transcription, each with its own typed exception
* **Segmentation** chunks large files so transcription scales to long recordings without timing out or exhausting memory, then stitches transcripts back together with corrected timestamps
* **Event-driven trigger** via `watchdog` reacts to new files immediately instead of polling on an interval, with a slow sweep only as a backstop for missed events
* **Structured, typed error handling** — every failure carries the stage and file it failed at; failed files land in `quarantine/` with an `.error.txt` sidecar instead of vanishing into a log no one reads

💡 Demonstrates **designing for how a system is actually used in production**, not just the happy path — every stage exists because of a specific real failure mode, not a generic best practice bolted on

**Tech:** Python, OpenAI Whisper, watchdog, pydub/ffmpeg, pytest

---

### 🌞 NeuroSpike — Solar Forecasting using AI + SNN

🔗 https://neuromorphic-solar-forecast.onrender.com

> A research-grade + production-ready AI system for solar energy forecasting

* Built full pipeline: **data → feature engineering → ML/DL → API → dashboard**
* Implemented **Spiking Neural Networks (SNN)** alongside LSTM
* Achieved **RMSE 29.67, R² 0.9877**, outperforming BiLSTM baseline
* Includes **power output estimation + savings calculator + city comparison**

💡 This is not just a model — it's a **complete deployable AI system**

**Tech:** Python, FastAPI, Streamlit, LSTM, SNN, ML Pipeline

---

### 🧠 One Answer Engine — AI Product Advisor

🔗 https://one-answer-engine-2.onrender.com

> Reasoning-first recommendation system (logic + AI explanation)

* Uses **deterministic scoring engine** before LLM
* AI explains decisions → builds **user trust**
* Bilingual system (English + Arabic)

💡 Demonstrates **AI system design + product thinking**

**Tech:** FastAPI, React, Groq (LLaMA 3), LLM Pipelines

---

### 📋 TaskFlow — Team Collaboration SaaS

🔗 https://team-task-manager-1-l6jn.onrender.com

> Full-stack production application with authentication & Kanban system

* JWT authentication + Role-Based Access Control (RBAC)
* Kanban board with real-time task management
* Fully deployed with PostgreSQL backend

💡 Demonstrates **backend engineering + system design**

**Tech:** React, FastAPI, PostgreSQL, Docker

---

### 🎨 Social Media Studio — GenAI Content Engine

> AI-powered Instagram content generator (idea → slides → export)

* Converts raw idea into structured multi-slide content
* Real-time preview + downloadable creatives

💡 Demonstrates **GenAI + UI/UX thinking**

**Tech:** Node.js, Express, Groq (LLaMA 3), HTML/CSS/JS

---

## 📂 Other Projects

| Project                          | Description                             | Stack                   |
| --------------------------------- | ---------------------------------------- | ------------------------ |
| 🧠 Employee Attrition Prediction  | ML classification + feature engineering  | Python, Scikit-Learn     |
| 📊 Customer Behavior Analysis     | End-to-end analytics pipeline            | Pandas, SQL              |
| 🎮 Hand Gesture Controller        | Real-time computer vision system         | OpenCV, MediaPipe        |
| 🗂️ Restaurant Scraper            | Automated web scraping pipeline          | Selenium, BeautifulSoup  |

---

## 💼 Experience

**🔹 AI Research Intern — Planto.ai**

* Worked on LLM workflows, prompt design, and evaluation
* Contributed to improving AI system reliability

**🔹 Vocational Trainee — BSNL**

* Learned telecom systems, monitoring, and fault detection

---

## 🛠️ Technical Skills

**Languages:** Python, SQL, Java, TypeScript

**Machine Learning:**
Scikit-Learn, XGBoost, Regression, Classification, CNN, LSTM, Transformers, SNN

**Generative AI:**
OpenAI API, Groq, Google Gemini, Prompt Engineering, Structured/JSON-Schema Outputs, LLM Evaluation, Whisper

**Backend:**
FastAPI, Node.js, Express, Event-Driven Systems (watchdog), zod

**Frontend:**
React, Next.js, HTML, CSS, JavaScript, Tailwind CSS

**Databases:**
PostgreSQL, MySQL

**Tools:**
Git, Docker, Jupyter, VS Code

---

## 📚 Currently Learning

* RAG pipelines & LangChain
* PyTorch (advanced deep learning)
* MLOps (Docker, MLflow)
* Cloud (AWS basics)

## 📬 Connect With Me

* 📧 Email: [Pragy34@gmail.com](mailto:Pragy34@gmail.com)
* 💼 LinkedIn: https://linkedin.com/in/pragy-upadhyay-893895246
* 💻 GitHub: https://github.com/pragy34

---

<div align="center">

*"Building real-world AI systems, not just models."*

</div>
