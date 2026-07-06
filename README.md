<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Sai%20Saran%20Tottempudi&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=36&desc=ML%20Engineer%20%C2%B7%20AI%20Engineer%20%C2%B7%20Data%20Engineer&descAlignY=58&descSize=18" width="100%"/>

<p align="center">
  MSc AI &amp; Data Analytics — Loughborough University London &nbsp;|&nbsp; BTech Computer Science (AI &amp; ML) — SRM University
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/tottempudi-sai-saran"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  &nbsp;
  <a href="mailto:tottempudisaisaran@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  &nbsp;
  <a href="https://orcid.org/0009-0007-3904-523X"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"/></a>
</p>

---

> Fifteen+ production systems shipped. Two IEEE publications. I don't stop at AUC — I calibrate, deploy, containerise, monitor, and retrain.

---

## What I Build

- **End-to-end MLOps platforms** — automated lifecycle: ingest → validate → train → register → serve → monitor → retrain (MLflow · Prefect · Evidently · XGBoost + SHAP · Docker Compose)
- **LLM & RAG systems** — production-grade, not prototypes (LangChain · ChromaDB · Ollama · Kubernetes · Helm · Terraform)
- **MCP servers & AI tooling** — Model Context Protocol integrations for Claude: RAG over knowledge bases, JD gap analysis, IaC security scanning
- **Statistical & ML models** — calibrated, governed, API-deployed (Poisson/Gamma GLMs · LightGBM · PyTorch LSTM · IsolationForest)
- **Cloud-native platforms** — full observability on free tiers (Oracle Cloud k3s · Grafana Cloud · GCP Cloud Functions · GitHub Actions · WIF keyless auth)

---

## Featured Projects

### [readmit-ai](https://github.com/saisarantottempudi/readmit-ai) — Hospital Readmission Risk, End-to-End MLOps
![CI](https://img.shields.io/badge/CI-passing-4caf50?style=flat-square) ![Stack](https://img.shields.io/badge/MLflow%20·%20Prefect%20·%20Evidently%20·%20XGBoost%20·%20SHAP-0194E2?style=flat-square)

Production-grade MLOps platform predicting 30-day hospital readmission risk — a tracked NHS metric (~£2.5B/yr). The full automated lifecycle most portfolio projects skip: pandera-validated ingest, XGBoost + SHAP training, governed MLflow registry with champion/challenger promotion, FastAPI serving with per-prediction explainability, Evidently drift detection that triggers retraining but can never silently degrade the champion. Eight containers, one `docker compose up`, $0, no cloud dependency.

---

### [QuantForge](https://github.com/saisarantottempudi/quantforge) — Language-Agnostic Backtesting Engine
![CI](https://img.shields.io/badge/CI-passing-4caf50?style=flat-square) ![Stack](https://img.shields.io/badge/FastAPI%20·%20WebSocket%20·%20Docker%20·%20Python%20%2F%20Go%20%2F%20TS-2196F3?style=flat-square)

Backtesting and paper trading engine where strategies live in *any* language — Python, Go, TypeScript, Rust, anything with WebSocket support. REST session management, streaming `BAR` events, order fills with configurable slippage and fees, and reports with Sharpe ratio, max drawdown, VaR, and equity curve. Example clients in three languages.

---

### [FinSight](https://github.com/saisarantottempudi/finsight) — Real-time Portfolio Risk & Fraud Analytics
![Stack](https://img.shields.io/badge/FastAPI%20·%20k3s%20·%20Grafana%20Cloud%20·%20IsolationForest-F46800?style=flat-square)

End-to-end fintech platform: VaR (95%/99%), Sharpe, volatility, max drawdown on live market data (yfinance → PostgreSQL), IsolationForest fraud scoring on every transaction, Streamlit dashboard. Deployed to an Oracle Cloud ARM k3s cluster via GitHub Actions + GHCR, with metrics, logs, and traces shipped to Grafana Cloud. Runs entirely on free tiers — $0.

---

### MCP Server Suite — Claude Integrations (Model Context Protocol)
![Stack](https://img.shields.io/badge/MCP%20·%20ChromaDB%20·%20BeautifulSoup%20·%20Python-8E44AD?style=flat-square)

Three local MCP servers built for real daily use with Claude Code:

- **[rag-profile-mcp](https://github.com/saisarantottempudi/rag-profile-mcp)** — embeds a personal knowledge base into ChromaDB; semantic search, JD matching, and skill lookup from natural language
- **[jd-gap-analyzer-mcp](https://github.com/saisarantottempudi/jd-gap-analyzer-mcp)** — scrapes job descriptions, extracts skills via a 150+ term tech taxonomy, and produces MATCH/PARTIAL/GAP reports with a 30-day study plan
- **[iac-explainer-mcp](https://github.com/saisarantottempudi/iac-explainer-mcp)** — Terraform/Dockerfile/Compose/K8s security scanning, resource extraction, and infra diffing

---

### [llmscope](https://github.com/saisarantottempudi/llmscope) — LLM Inference Benchmarking
![Stack](https://img.shields.io/badge/Anthropic%20·%20OpenAI%20·%20Ollama%20·%20CLI-EE4C2C?style=flat-square)

Benchmarks what actually matters in production LLM serving: time-to-first-token, p50/p95/p99 latency, tokens/sec throughput, and cost per inference — across Anthropic, OpenAI, and local Ollama models, with concurrent load testing. One command, provider-comparable reports.

---

### [MICKEY](https://github.com/saisarantottempudi/MICKEY) — Fully Local AI Assistant
![Stack](https://img.shields.io/badge/Ollama%20·%20Flask%20·%20React%2019%20·%20Three.js-61DAFB?style=flat-square)

Jarvis-inspired voice assistant running 100% locally on Apple Silicon — no data leaves the hardware. Wake-word + push-to-talk voice, macOS system control, conversation memory, smart model routing (3B fast path / 8B complex), Three.js HUD, cross-device access via Tailscale, and a plugin system.

---

### [DocuMind](https://github.com/saisarantottempudi/documind) — Production RAG Document Q&A
![CI](https://img.shields.io/badge/CI-passing-4caf50?style=flat-square) ![Tests](https://img.shields.io/badge/tests-25%2F25-4caf50?style=flat-square) ![Stack](https://img.shields.io/badge/Kubernetes%20·%20Helm%20·%20Terraform%20·%20Prometheus-326CE5?style=flat-square)

FastAPI + LangChain 0.3 + ChromaDB + Redis + Ollama (llama3.2). Deployed to k3d with HPA (2–8 replicas), NetworkPolicy zero-trust, PodDisruptionBudget, and ResourceQuota. Full IaC via Terraform. CI/CD: ruff → mypy → pytest → GHCR → Trivy CVE scan → SARIF → Helm deploy → smoke test.

---

### [SupportIQ](https://github.com/saisarantottempudi/supportiq) — AI Customer Support Triage Platform
![CI](https://img.shields.io/badge/CI-passing-4caf50?style=flat-square) ![Stack](https://img.shields.io/badge/FastAPI%20·%20Claude%20API%20·%20Celery%20·%20React-009688?style=flat-square)

Claude classifies every ticket (category, priority, sentiment, confidence) and drafts a 150–250 word reply — asynchronously via Celery so the API returns in < 50ms. React 18 + TypeScript frontend with charts and a ticket detail view. Debugged 9 real CI issues (asyncpg loop isolation, bcrypt version conflict, BaseHTTPMiddleware ASGI conflict) to reach a clean green pipeline.

---

### [Healthcare Claims GLM](https://github.com/saisarantottempudi/healthcare-claims-glm) — Insurance Pricing Model
![Tests](https://img.shields.io/badge/tests-77-4caf50?style=flat-square) ![Gini](https://img.shields.io/badge/Gini-0.60-2196F3?style=flat-square) ![Stack](https://img.shields.io/badge/statsmodels%20·%20MLflow%20·%20Docker-FF6F00?style=flat-square)

Poisson GLM (frequency) × Gamma GLM (severity) = Pure Premium — the actuarial two-part model used by Aviva, AXA, BUPA. 50k synthetic UK policyholders. FastAPI + batch endpoint, MLflow tracking, 11 publication-quality evaluation figures (Lorenz curves, calibration by decile, residual plots). *Shows when not to use gradient boosting.*

---

## More Projects

| Project | What it is | Stack |
|---|---|---|
| [Credit Risk Profit Engine](https://github.com/saisarantottempudi/credit_risk_profit_engine) | Calibrated PD → Expected Loss → risk-based APR decisioning; isotonic calibration cut Brier from 0.156 → 0.062 | LightGBM · FastAPI |
| [F1 Analytics AI](https://github.com/saisarantottempudi/f1_analytics) | 8-stage ML platform: LSTM race predictor, RL pit strategy, Monte Carlo simulator, RAG layer | PyTorch · RL · ChromaDB · Streamlit |
| [F1 AI Strategy Engine](https://github.com/saisarantottempudi/f1_ai_strategy_engine) | Pit-stop strategy optimization with lap-time ML + Monte Carlo under uncertainty | FastF1 · FastAPI |
| [Serverless Image Recognition](https://github.com/saisarantottempudi/serverless_image_rec) | GCS → Cloud Function Gen2 → TFLite inference → GPT-4o-mini captioning; keyless WIF deploys | GCP · TFLite · GitHub Actions |
| [Telugu Text Summarization](https://github.com/saisarantottempudi/telugu-text-summarization) | mBERT vs T5 vs XLNet for low-resource extractive summarization — BLEU 0.456 / ROUGE-1 0.72 | HuggingFace · NLP |
| [MSc RL Recipe Optimizer](https://github.com/saisarantottempudi/msc-rl-recipe-optimizer) | PPO agent for ingredient optimisation with VAE, RAG, and LLM integration | PPO · ChromaDB · GPT-4o / Claude |
| [Customer Churn Prediction](https://github.com/saisarantottempudi/customer-churn-prediction) | Production-ready churn prediction and retention recommendation system | scikit-learn · FastAPI |

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
![XGBoost](https://img.shields.io/badge/XGBoost-EB4C2C?style=flat-square)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)

**MLOps & Infrastructure**  
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Prefect](https://img.shields.io/badge/Prefect-070E10?style=flat-square&logo=prefect&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

**Cloud & Frontend**  
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Oracle Cloud](https://img.shields.io/badge/Oracle_Cloud-F80000?style=flat-square&logo=oracle&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>

<!---
saisarantottempudi/saisarantottempudi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->
