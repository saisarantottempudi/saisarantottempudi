<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Sai%20Saran%20Tottempudi&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=36&desc=ML%20Engineer%20%C2%B7%20AI%20Engineer%20%C2%B7%20Data%20Engineer&descAlignY=58&descSize=18" width="100%"/>

<p align="center">
  MSc AI &amp; Data Analytics — Loughborough University London &nbsp;|&nbsp; BSc Computer Science (AI &amp; ML) — SRM University
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/saisarantottempudi"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  &nbsp;
  <a href="mailto:saisarant28@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  &nbsp;
  <a href="https://orcid.org/0009-0007-3904-523X"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"/></a>
</p>

---

> Eight production systems shipped. Two IEEE publications. I don't stop at AUC — I calibrate, deploy, containerise, and monitor.

---

## What I Build

- **LLM & RAG systems** — production-grade, not prototypes (LangChain · ChromaDB · Ollama · Kubernetes · Helm · Terraform)
- **Statistical & ML models** — calibrated, governed, API-deployed (Poisson/Gamma GLMs · LightGBM · PyTorch LSTM)
- **AI-powered full-stack apps** — async Python + React, real CI pipelines, background task queues (FastAPI · Celery · Claude API)
- **Cloud-native ML pipelines** — serverless and containerised (GCP Cloud Functions · Docker · GitHub Actions · WIF keyless auth)

---

## Featured Projects

### [DocuMind](https://github.com/saisarantottempudi/documind) — Production RAG Document Q&A
![CI](https://img.shields.io/badge/CI-passing-4caf50?style=flat-square) ![Tests](https://img.shields.io/badge/tests-25%2F25-4caf50?style=flat-square) ![Stack](https://img.shields.io/badge/Kubernetes%20·%20Helm%20·%20Terraform%20·%20Prometheus-326CE5?style=flat-square)

FastAPI + LangChain 0.3 + ChromaDB + Redis + Ollama (llama3.2). Deployed to k3d with HPA (2–8 replicas), NetworkPolicy zero-trust, PodDisruptionBudget, and ResourceQuota. Full IaC via Terraform. CI/CD: ruff → mypy → pytest → GHCR → Trivy CVE scan → SARIF → Helm deploy → smoke test.

---

### [SupportIQ](https://github.com/saisarantottempudi/supportiq) — AI Customer Support Triage Platform
![CI](https://img.shields.io/badge/CI-passing-4caf50?style=flat-square) ![Stack](https://img.shields.io/badge/FastAPI%20·%20Claude%20API%20·%20Celery%20·%20React-009688?style=flat-square)

Claude haiku-4-5 classifies every ticket (category, priority, sentiment, confidence) and drafts a 150–250 word reply — asynchronously via Celery so the API returns in < 50ms. React 18 + TypeScript frontend with charts and a ticket detail view. Debugged 9 real CI issues (asyncpg loop isolation, bcrypt version conflict, BaseHTTPMiddleware ASGI conflict) to reach a clean green pipeline.

---

### [Healthcare Claims GLM](https://github.com/saisarantottempudi/healthcare-claims-glm) — Insurance Pricing Model
![Tests](https://img.shields.io/badge/tests-77-4caf50?style=flat-square) ![Gini](https://img.shields.io/badge/Gini-0.60-2196F3?style=flat-square) ![Stack](https://img.shields.io/badge/statsmodels%20·%20MLflow%20·%20Docker-FF6F00?style=flat-square)

Poisson GLM (frequency) × Gamma GLM (severity) = Pure Premium — the actuarial two-part model used by Aviva, AXA, BUPA. 50k synthetic UK policyholders. FastAPI + batch endpoint, MLflow tracking, 11 publication-quality evaluation figures (Lorenz curves, calibration by decile, residual plots). *Shows when not to use gradient boosting.*

---

### [Credit Risk Profit Engine](https://github.com/saisarantottempudi/credit_risk_profit_engine) — ML Decisioning System
![Stack](https://img.shields.io/badge/LightGBM%20·%20Calibration%20·%20FastAPI-EF5350?style=flat-square)

LightGBM champion vs. Logistic Regression baseline. Isotonic calibration brings raw PD from 0.156 → 0.062 (Brier Score improvement). Decision engine: PD → Expected Loss (PD × LGD × EAD) → risk-based APR → Expected Profit → Approve/Reject. Medallion data architecture. FastAPI scoring endpoint.

---

### [F1 Analytics AI](https://github.com/saisarantottempudi/f1_analytics) — Full ML Platform (8 Stages)
![Stack](https://img.shields.io/badge/PyTorch%20LSTM%20·%20RL%20·%20Monte%20Carlo%20·%20RAG%20·%20Streamlit-EE4C2C?style=flat-square)

LSTM race predictor + Tabular-Q RL pit strategy agent + Monte Carlo lap simulator + RAG layer (ChromaDB + MiniLM + Claude Haiku) + FastAPI backend + Streamlit frontend with Plotly lap-replay animation. Real data: FastF1 (2022–2025) + Ergast (1950–present). MPS-accelerated on Apple Silicon.

---

### [Serverless Image Recognition](https://github.com/saisarantottempudi/serverless_image_rec) — GCP Event-Driven Pipeline
![Stack](https://img.shields.io/badge/GCP%20Cloud%20Functions%20·%20TFLite%20·%20OpenAI%20·%20WIF-4285F4?style=flat-square)

GCS image upload → Cloud Function Gen2 → MobileNetV2 TFLite inference → OpenAI GPT-4o-mini caption → JSON result back to GCS. Deployed via GitHub Actions with Workload Identity Federation — no long-lived service account keys in secrets.

---

### [Telugu Text Summarization](https://github.com/saisarantottempudi/telugu-text-summarization) — NLP Research
![BLEU](https://img.shields.io/badge/BLEU-0.456-9C27B0?style=flat-square) ![ROUGE](https://img.shields.io/badge/ROUGE--1-0.72-9C27B0?style=flat-square)

Compared mBERT, T5, and XLNet for extractive summarization of Telugu Wikipedia (~80M speakers, low-resource language). mBERT (BLEU 0.456 / ROUGE-1 0.72) outperformed English-only models by 6×, confirming multilingual pretraining dominates architecture choice for low-resource NLP tasks. Undergraduate capstone project.

---

## Research Publications

| Paper | Venue | DOI |
|---|---|---|
| Analyzing the Health Data: An Application of High Utility Itemset Mining | IEEE ICAICCIT 2023 | [10.1109/ICAICCIT60255.2023.10466177](https://ieeexplore.ieee.org/document/10466177) |
| Evaluation of Asymmetric Link-Based AODV-RPL for LLNs in COOJA Simulator | IEEE IC2E3 2024 | [10.1109/ic2e362166.2024.10826896](https://ieeexplore.ieee.org/document/10826896) |

---

## Tech Stack

**Core**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**ML / AI**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)

**Infrastructure**  
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

**Cloud & Frontend**  
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>

<!---
saisarantottempudi/saisarantottempudi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->
