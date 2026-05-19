# Sai Saran Tottempudi

**ML Engineer · AI Engineer · Data Engineer**  
MSc Artificial Intelligence & Data Analytics — Loughborough University London  
BSc Computer Science (AI & ML) — SRM University

I build production-grade ML and data systems end-to-end — from model to API to Kubernetes to CI/CD. Eight shipped projects, two IEEE publications, targeting roles in the UK and EU.

---

## Projects

### DocuMind — Production RAG Document Q&A
**[github.com/saisarantottempudi/documind](https://github.com/saisarantottempudi/documind)** · CI green · 25/25 tests

End-to-end RAG system: FastAPI · LangChain 0.3 · ChromaDB · Redis · Ollama (llama3.2) · Docker Compose · Kubernetes (HPA, NetworkPolicy, PDB) · Helm · Terraform · Prometheus/Grafana · GitHub Actions (Trivy, GHCR, Codecov, SARIF)

> Full DevOps + MLOps lifecycle — local dev → containerised → k8s-deployed → monitored → hardened. Strongest portfolio artifact for MLOps/Platform Engineer roles.

---

### SupportIQ — AI Customer Support Triage Platform
**[github.com/saisarantottempudi/supportiq](https://github.com/saisarantottempudi/supportiq)** · CI green (lint · tests · frontend build)

Full-stack AI engineering project: FastAPI async · SQLAlchemy 2.0 + asyncpg · Celery + Redis · Anthropic Claude haiku-4-5 (classification + draft responses) · React 18 + TypeScript + Tailwind · Docker Compose · JWT auth · GitHub Actions CI

> Automates ticket triage with Claude AI. Ticket creation returns in < 50ms; AI runs in the background via Celery. Debugged 9 real CI issues to get to green.

---

### Healthcare Claims GLM — Insurance Pricing Model
**[github.com/saisarantottempudi/healthcare-claims-glm](https://github.com/saisarantottempudi/healthcare-claims-glm)** · 77 tests

Poisson GLM (frequency) × Gamma GLM (severity) = Pure Premium — the actuarial two-part model used by Aviva, AXA, BUPA. Gini 0.60 on 50k synthetic policyholders. statsmodels · MLflow · FastAPI + batch endpoint · Docker multi-stage · GitHub Actions CI

> Shows when *not* to use gradient boosting. Directly relevant to regulated-sector DS interviews.

---

### Credit Risk Profit Engine
**[github.com/saisarantottempudi/credit_risk_profit_engine](https://github.com/saisarantottempudi/credit_risk_profit_engine)**

LightGBM champion + Logistic Regression baseline with isotonic calibration. Decision engine: PD → Expected Loss → risk-based APR → Expected Profit → Approve/Reject. Medallion data architecture. FastAPI scoring endpoint. Home Credit Kaggle dataset.

---

### F1 Analytics AI — Full ML Platform
**[github.com/saisarantottempudi/f1_analytics](https://github.com/saisarantottempudi/f1_analytics)** · 8 stages complete

PyTorch LSTM race prediction · RL pit strategy agent · Monte Carlo lap simulation · RAG layer (ChromaDB + MiniLM + Claude Haiku) · FastAPI backend · Streamlit frontend with Plotly lap-replay animation. Real data: FastF1 (2022–2025) + Ergast (1950–present).

---

### F1 AI Strategy Engine — Terminal-First CLI
**[github.com/saisarantottempudi/f1_ai_strategy_engine](https://github.com/saisarantottempudi/f1_ai_strategy_engine)**

Bronze → Silver → Gold medallion pipeline on FastF1 data. Scikit-learn regression for next-lap time. Monte Carlo pit-window simulator with risk scores. FastAPI + shell CLI. No GUI dependency.

---

### Serverless Image Recognition — GCP Cloud Functions
**[github.com/saisarantottempudi/serverless_image_rec](https://github.com/saisarantottempudi/serverless_image_rec)**

Event-driven: GCS upload → Cloud Function Gen2 → MobileNetV2 TFLite inference → OpenAI GPT caption → JSON result back to GCS. Deployed via GitHub Actions with Workload Identity Federation (keyless auth, no long-lived secrets).

---

### Telugu Text Summarization — NLP Research
**[github.com/saisarantottempudi/telugu-text-summarization](https://github.com/saisarantottempudi/telugu-text-summarization)** · Undergraduate capstone

Compared mBERT, T5, XLNet for extractive summarization of Telugu Wikipedia (566 articles). mBERT: BLEU 0.456 / ROUGE-1 0.72 — outperformed English-only models by 6×, confirming multilingual pretraining dominates architecture for low-resource NLP.

---

## Research Publications

| Paper | Venue | DOI |
|---|---|---|
| Analyzing the Health Data: An Application of High Utility Itemset Mining | IEEE ICAICCIT 2023 | [10.1109/ICAICCIT60255.2023.10466177](https://ieeexplore.ieee.org/document/10466177) |
| Evaluation of Asymmetric Link-Based AODV-RPL for LLNs in COOJA Simulator | IEEE IC2E3 2024 | [10.1109/ic2e362166.2024.10826896](https://ieeexplore.ieee.org/document/10826896) |

---

## Tech Stack

**Core**  
Python · FastAPI · Pydantic v2 · SQLAlchemy 2.0 · asyncpg · pytest

**ML / AI**  
PyTorch · HuggingFace Transformers · scikit-learn · LightGBM · statsmodels · MLflow · LangChain 0.3 · RAG · ChromaDB · sentence-transformers · Anthropic Claude API · OpenAI API

**Infrastructure**  
Docker · Kubernetes · Helm · Terraform · GitHub Actions · Prometheus · Grafana · Trivy

**Data**  
PostgreSQL · Redis · Celery · Medallion architecture · Parquet · openpyxl

**Cloud**  
GCP (Cloud Functions Gen2 · GCS · Eventarc · Workload Identity Federation)

**Frontend**  
React 18 · TypeScript · Tailwind CSS · Streamlit · Plotly

---

## Links

[LinkedIn](https://www.linkedin.com/in/saisarantottempudi) · [Email](mailto:saisarant28@gmail.com)

<!---
saisarantottempudi/saisarantottempudi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->
