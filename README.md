<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=170&section=header&text=Anupam%20Kumar&fontSize=46&fontColor=ffffff&fontAlignY=38&desc=AI%20Engineer%20%E2%80%A2%20Agentic%20Systems%20%E2%80%A2%20Backend%20Platforms&descAlignY=58&descSize=16&descColor=a78bfa" />

<a href="https://anupai-portfolio.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>&nbsp;
<a href="https://www.linkedin.com/in/anupam-kumar-142931253/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>&nbsp;
<a href="https://github.com/anupamkr1708"><img src="https://img.shields.io/badge/GitHub-161b22?style=for-the-badge&logo=github&logoColor=white" /></a>&nbsp;
<a href="mailto:anupsharma1708@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>&nbsp;
<img src="https://komarev.com/ghpvc/?username=anupamkr1708&color=7c3aed&style=for-the-badge&label=PROFILE+VIEWS" />

</div>

<br/>

## About

I'm Anupam Kumar, an AI Engineer and Computer Science graduate from **IIITM Gwalior ('25)**. I build **production-oriented AI systems** across **RAG, agentic workflows, retrieval, computer vision, and AI backends**.

My focus is on making AI systems **reliable beyond the demo** — from retrieval and grounding to evaluation, backend architecture, and deployment.

Currently open to **AI Engineering, ML/AI Infrastructure, and Platform Engineering** roles.


*Always interested in working with people who think deeply, build seriously, and aren't afraid to challenge how something is supposed to be done.*

<br/>

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**AI / LLM**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square) ![RAG](https://img.shields.io/badge/RAG-7c3aed?style=flat-square) ![Agentic AI](https://img.shields.io/badge/Agentic%20AI-7c3aed?style=flat-square)

**Retrieval & Vector Search**

![FAISS](https://img.shields.io/badge/FAISS-4b5563?style=flat-square) ![Pinecone](https://img.shields.io/badge/Pinecone-1a1a2e?style=flat-square) ![ChromaDB](https://img.shields.io/badge/ChromaDB-4b5563?style=flat-square) ![BM25](https://img.shields.io/badge/BM25-4b5563?style=flat-square)

**Backend & Data**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)

**DevOps, Cloud & Observability**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)


<br/>

## Featured Projects

### 1. AetherCV — Graph-RAG Research Engine
**A citation-graph-aware retrieval system for computer vision research — dense, lexical, and citation-graph signals fused into a single retrieval layer, with grounding measured rather than assumed.**

Most RAG systems treat retrieval as one similarity search. AetherCV treats it as three independent evidence sources — semantic similarity, exact terminology via BM25, and citation relationships between papers — merged through a router that decides which signal to trust for a given question, then verifies the answer is actually supported before it's returned.

- Multi-signal retrieval (dense + BM25 + citation-graph) reaches **0.94 context recall**, measured against a held-out evaluation set rather than reported from a single run.
- A **7-layer Redis caching architecture** (exact, semantic, retrieval, decomposition, intent) pushes the **cache hit rate above 84%**, holding **p99 latency near 4.9 seconds on CPU-only infrastructure** — no GPU in the serving path.
- A multi-signal semantic router (domain centroid, retrieval-support probe, entity-shape check) catches out-of-domain questions *before* generation, keeping every answered response grounded in retrieved evidence with zero false-positive escapes.
- Fully instrumented for MLOps — MLflow experiment tracking, Prometheus/Grafana monitoring, containerized deployment — with zero evaluation failures across all benchmark runs.

`Python` `FastAPI` `FAISS` `BM25` `Redis` `PostgreSQL` `Prometheus` `MLflow` `Docker`

**[Live Demo](https://aether-cv.vercel.app/) · [GitHub](https://github.com/anupamkr1708/AetherCV-Graph-RAG)**

<br/>

### 2. LeadBoost — B2B Lead Intelligence Platform
**A single natural-language query — *"electronics stores in Bengaluru"* — becomes validated, AI-scored leads with drafted outreach, end to end, in one API call.**

At its core is a **six-stage identity resolution engine** solving a problem most lead-gen tools quietly get wrong: confirming a website actually belongs to *this* business, in *this* location — not a same-named competitor three cities over, or an unrelated directory listing. Evidence, features, and five independent verifiers feed a confidence-propagation model, so every match ships with an explainable score instead of a guess.

- Benchmarked on **113 real-world queries across 20+ Indian cities**: **88.8%** correct website resolution, **87.4%** validation success, **96.4%** cross-provider agreement, **100%** query-parse reliability.
- A **six-tier escalating scraper** (static fetch → TLS-fingerprint impersonation → headless rendering → multi-page crawl) feeds a three-tier enrichment waterfall and **four LangGraph-orchestrated agents** — Company Intelligence, Decision, Review, Messaging — each backed by a deterministic fallback, so no stage depends on an LLM to function.
- Grounding is independently measured, not assumed: an evaluation harness runs the full production pipeline end to end, cross-checking every AI-claimed signal against scraped evidence before it reaches a lead record. The Decision agent can only **downgrade** a lead's priority, never inflate it; outreach falls back to strict templates rather than let a model invent facts.

`FastAPI` `SQLAlchemy` `LangGraph` `LangChain` `Groq (Llama 3.3 70B)` `Playwright` `curl_cffi` `Next.js 14` `TypeScript` `TanStack Query` `Zustand` `Prometheus / Grafana`

**[Live Demo](https://lead-boost-saas.vercel.app/) · [GitHub](https://github.com/anupamkr1708/LeadBoost-saas)**

<br/>

### Other Projects

**AyurGenix** — Agentic RAG over 10,000+ pages of Sanskrit manuscripts. Custom Char-CNN OCR for Sanskrit script, Pinecone-indexed sub-second retrieval, cross-encoder reranking, and citation-grounded answers via a LLaMA-3 conversational layer.
`FastAPI` `PyTorch` `Pinecone` `LangChain` — [GitHub](https://github.com/anupamkr1708/AyurProject)

**TalentForge AI** — Autonomous job-application pipeline: LinkedIn scraping → LLM resume scoring (70% semantic, 30% keyword) → Playwright-based Easy Apply, gated by a strict state machine and a 4-tier LLM fallback chain for unattended, reliable operation.
`Python` `Playwright` `Groq` `LangChain` `Streamlit` — [GitHub](https://github.com/anupamkr1708/TalentForge-AI)

<br/>

## GitHub Activity

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=anupamkr1708&show_icons=true&theme=tokyonight&include_all_commits=false&count_private=true&hide_border=true&bg_color=0d1117&title_color=7c3aed&icon_color=a78bfa&text_color=c9d1d9"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anupamkr1708&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=7c3aed&text_color=c9d1d9"/>

<br/>

![](https://github-readme-streak-stats.herokuapp.com/?user=anupamkr1708&theme=tokyonight&hide_border=true&background=0d1117&ring=7c3aed&fire=a78bfa&currStreakLabel=a78bfa&mode=weekly)

<br/>

![](https://github-readme-activity-graph.vercel.app/graph?username=anupamkr1708&theme=tokyo-night&hide_border=true&area=true&bg_color=0d1117&color=a78bfa&line=7c3aed&point=ffffff&days=365&custom_title=Contribution%20Activity%20(Last%2012%20Months))

</div>

<br/>

## Education

**Indian Institute of Information Technology and Management, Gwalior**
B.Tech in Computer Science — 2021 to 2025

<br/>

<div align="center">

📧 **[Email](mailto:anupsharma1708@gmail.com)** &nbsp;·&nbsp; 💼 **[LinkedIn](https://www.linkedin.com/in/anupam-kumar-142931253/)** &nbsp;·&nbsp; 🌐 **[Portfolio](https://anupai-portfolio.vercel.app/)** &nbsp;·&nbsp; 🐙 **[GitHub](https://github.com/anupamkr1708)**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=100&section=footer" />

</div>
