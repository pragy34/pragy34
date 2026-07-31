<div align="center">

# Hi, I'm Pragy Upadhyay 👋

**AI Engineer · Machine Learning · Backend Systems · Data Analytics**

Building production-grade AI applications with FastAPI, React, LLMs, SQL, and Cloud.

<p align="center">
<a href="https://github.com/pragy34"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://linkedin.com/in/pragy-upadhyay-893895246"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:pragy34@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

![Profile views](https://komarev.com/ghpvc/?username=pragy34&color=blue)

</div>

---

## 📌 Highlights

* Built and **deployed 5+ production AI/full-stack applications** — live, not just localhost
* **26 automated tests** and **10 documented security fixes** on a live equity-research platform (MarketLens)
* End-to-end SQL → BI analytics warehouse diagnosing **$406K in inventory bleed** across 500 SKUs (IHDAP)
* Hands-on with **LLM pipelines** — structured/JSON-schema outputs, prompt engineering, multi-provider fallback (Groq, Gemini)
* Deep learning research: **SNN + LSTM solar forecasting**, RMSE 29.67, R² 0.9877 — self-caught and fixed a data-leakage bug pre-submission
* Full-stack: **FastAPI / Express + React / Next.js + PostgreSQL / SQLite**, deployed on Render, Vercel, Railway

## 🎯 Open to Opportunities

`AI Engineer` · `Machine Learning Engineer` · `Data Analyst` · `Backend Developer` · `Full-Stack AI Engineer`

---

## 🛠️ Tech Stack

<p align="center">
<img src="https://skillicons.dev/icons?i=python,java,ts,react,nextjs,nodejs,fastapi,express,postgres,mysql,sqlite,docker,git,github,linux,tensorflow,pytorch,vercel"/>
</p>

**Data & BI:** SQL (CTEs, window functions, SCD Type 2) · Power BI (DAX) · Tableau (LOD) · Excel (OpenPyXL)
**Generative AI:** OpenAI API · Groq · Google Gemini · Prompt Engineering · Structured Outputs · Whisper
**ML/DL:** Scikit-Learn, XGBoost, CNN, LSTM, Transformers, SNN

---

## 📊 GitHub Stats

<p align="center">
<img src="https://github-readme-stats.vercel.app/api?username=pragy34&show_icons=true&theme=tokyonight" height="165"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=pragy34&layout=compact&theme=tokyonight" height="165"/>
</p>

<p align="center">
<img src="https://streak-stats.demolab.com?user=pragy34&theme=tokyonight"/>
</p>

---

## 🏆 Featured Projects

### 1. 📈 MarketLens — Live NSE Equity Research Terminal

**Production-grade equity research platform** — screening, peer valuation, sector heatmaps, portfolio analytics

**Tech:** Python · FastAPI · yfinance · SQLite · Chart.js · Vercel · Render

**Highlights**
✔ Live, split-deployed app (Render API + Vercel frontend) — not a demo
✔ 26 automated tests (backend mocked, frontend jsdom)
✔ 10 documented security fixes — XSS, session-ID leakage, open CORS, unbounded input, event-loop blocking
✔ Diagnosed and fixed a live sort-logic regression + a syntax bug that broke the whole frontend
✔ Portfolio analytics: XIRR (Newton-Raphson, no scipy), CSV validation, sector allocation

**Links:** [Live Demo](https://market-iq-real-time-stock-research.vercel.app) · [API](https://marketiq-real-time-stock-research-3vw4.onrender.com/api/status) · [Repo](https://github.com/pragy34/MarketIQ-Real-Time-Stock-Research-Portfolio-Analytics-Platform)

---

### 2. 📥 csv2crm — AI-Powered CRM CSV Importer

**LLM-based CSV-to-CRM schema mapper** — handles any leads export layout automatically

**Tech:** Next.js 14 · TypeScript · Express · zod · Groq · Google Gemini

**Highlights**
✔ Single source-of-truth schema drives the prompt, the JSON schema, and the zod validator — can't drift out of sync
✔ Groq primary / Gemini fallback behind a common AI-provider interface
✔ Concurrency-capped batch processing with exponential-backoff retries
✔ Real-time progress via Server-Sent Events, not a simulated timer
✔ Zero AI cost until the user confirms the client-side preview

**Links:** [Live Demo](https://csv2crm.vercel.app) · [API](https://csv2crm.onrender.com) · [Repo](https://github.com/pragy34/csv2crm)

---

### 3. 📦 IHDAP — Inventory Health Diagnostic & Action Playbook

**SQL → BI analytics project** diagnosing $406K in annual inventory bleed across 500 SKUs

**Tech:** Python · SQL (SQLite) · Power BI (DAX) · Tableau (LOD) · Excel (OpenPyXL)

**Highlights**
✔ Star-schema warehouse, 8 fact/dim tables, SCD Type 2 cost history
✔ 15 SQL queries (CTEs, window functions, full-outer-join emulation)
✔ Same numbers carried through Excel, Power BI, and Tableau
✔ One of 4 hypotheses tested was wrong — the correction redirected budget from markdown campaigns to stockout prevention on the top 10 SKUs
✔ Ends in a budget-constrained recovery plan ($50K → ~$35K/yr recovered), not just a dashboard

**Links:** [Repo](https://github.com/pragy34/ihdap)

---

### 4. 🎙️ Audio Transcription Pipeline — Resilient Event-Driven Whisper System

**Production-minded transcription pipeline** built after watching a naive "just call Whisper" approach fail silently

**Tech:** Python · OpenAI Whisper · watchdog · pydub/ffmpeg · pytest

**Highlights**
✔ Format detection by file bytes (`libmagic`), not filename trust
✔ Validation gate rejects corrupt/oversized/silent audio before it hits transcription
✔ Segmentation + timestamp-corrected stitching for long recordings
✔ Event-driven trigger (`watchdog`) with a slow-sweep backstop for missed events
✔ Every failure is typed, staged, and quarantined with an error sidecar — nothing vanishes into a log

**Links:** [Repo](https://github.com/pragy34/audio-transcription-pipeline)

---

### 5. 🌞 NeuroSpike — Solar Forecasting with LSTM + Spiking Neural Networks

**Research-grade + deployable AI system** for solar irradiance forecasting

**Tech:** Python · FastAPI · Streamlit · LSTM · SNN (snntorch)

**Highlights**
✔ Full pipeline: data → feature engineering → ML/DL → API → dashboard
✔ Best model (SNN) beat the BiLSTM baseline: **RMSE 29.67 vs 45.52, R² 0.9877 vs 0.971**
✔ Self-caught a data-leakage bug mid-project (`clearness_index` was mathematically equivalent to the target) — fixed and fully revalidated before submission
✔ Trained on NASA POWER hourly data (2021–2023) across 10 global cities
✔ Includes power-output estimation, savings calculator, and city comparison

**Links:** [Live Demo](https://neuromorphic-solar-forecast.onrender.com)

---

## 📂 More Projects

| Project                          | Description                                          | Stack                        |
| --------------------------------- | ----------------------------------------------------- | ----------------------------- |
| 🧠 One Answer Engine             | Deterministic scoring engine + LLM explanation layer, bilingual (EN/AR) | FastAPI, React, Groq (LLaMA 3) |
| 📋 TaskFlow                      | Team SaaS — JWT auth, RBAC, Kanban, PostgreSQL       | React, FastAPI, PostgreSQL, Docker |
| 🎨 Social Media Studio           | GenAI Instagram content engine (idea → slides → export) | Node.js, Express, Groq        |
| 🧠 Employee Attrition Prediction | ML classification + feature engineering              | Python, Scikit-Learn          |
| 📊 Customer Behavior Analysis    | End-to-end analytics pipeline                        | Pandas, SQL                   |
| 🎮 Hand Gesture Controller       | Real-time computer vision system                     | OpenCV, MediaPipe             |
| 🗂️ Restaurant Scraper           | Automated web scraping pipeline                      | Selenium, BeautifulSoup       |

---

## 💼 Experience

**🔹 AI Research Intern — Planto.ai**
Worked on LLM workflows, prompt design, and evaluation; contributed to improving AI system reliability.

**🔹 Vocational Trainee — BSNL**
Learned telecom systems, monitoring, and fault detection.

---

## 📚 Currently Learning

RAG pipelines, Fine-Tuning & Agentic frameworks (LangGraph, CrewAI) · Transformer architectures (attention, from-scratch) · PyTorch (advanced) · MLOps (Docker, MLflow) · AWS basics

---

## 📬 Connect With Me

<p align="center">
<a href="https://github.com/pragy34"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://linkedin.com/in/pragy-upadhyay-893895246"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:pragy34@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

<div align="center">

*"Building real-world AI systems, not just models."*

</div>
