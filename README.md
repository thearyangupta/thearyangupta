# Hi, I'm Aryan Gupta 👋

Applied AI Engineer building production-ready RAG systems, LLM agents, and backend infrastructure with Python, FastAPI, and LangGraph.

I don't just prototype — I ship. All four projects below are live, deployed, and evaluated with real metrics.

---

### 🚀 Featured Projects

**[GovPrep — AI Study Assistant (RAG + Agent)](https://github.com/thearyangupta/govprep)**
Source-cited RAG assistant for UPSC/CDS/SSC exam prep, grounded only in NCERT study material — explicitly returns "not in my sources" instead of hallucinating.
- Hybrid retrieval (PostgreSQL full-text + pgvector, fused via RRF), LangGraph ReAct agent, conversation memory
- Scored against a 24-question gold set: **Hit Rate@3: 0.375, MRR: 0.243, Faithfulness: 4.30/5**
- Deployed on Google Cloud Run · CI via GitHub Actions (pytest + ruff)
- 🔗 [Live demo](https://govprep-frontend-64960261938.asia-south1.run.app/)

**[FlowPilot AI — AI Workflow Automation Platform](https://github.com/thearyangupta/flowpilot-ai)**
Production-style platform connecting Gmail and a knowledge base: classifies incoming emails, drafts grounded replies, and holds them for human approval before sending.
- Idempotent execution, retries with exponential backoff + jitter, checkpoint recovery, full audit trails
- MCP server/client for permissioned tool access · Langfuse tracing for latency and token-cost observability
- Verified end-to-end with a real Gmail workflow in production
- 🔗 [Live demo](https://flowpilot-ai.site/)

**[Fraud Risk Intelligence Engine](https://github.com/thearyangupta/fraud-risk-intelligence-engine)**
An end-to-end fraud-risk pipeline built around temporal correctness and leakage prevention, not just predictive accuracy — chronological (not random) train/val/test splits, point-in-time behavioral features, and a frozen, validation-selected decision policy evaluated once on held-out test data.
- Compared rule-based, logistic regression, XGBoost, and Isolation Forest models — selected XGBoost (v3) for best PR-AUC (0.5173) and recall (0.9305)
- Held-out test: **ROC-AUC 0.9731, Recall 0.9417** — locked ALLOW/REVIEW/BLOCK policy routed 1,067 of 1,133 fraud transactions to REVIEW or BLOCK
- Dedicated regression test guards against feature leakage · CI runs tests + lint on every push
- Served locally via FastAPI (`/predict`) reusing the same offline feature/scoring/decision logic
- 🔗 [Repo](https://github.com/thearyangupta/fraud-risk-intelligence-engine)

**[Reading the Signals — Gemini-Powered Reflection Journal](https://github.com/thearyangupta/reading-the-signals)**
A private journaling app that reads across past entries to surface contradictions and reflect patterns back as a question, not a verdict. Built for Google Cloud's Gen AI Ideathon.
- Gemini API for reflection generation, Firebase Auth + Firestore for private per-user storage
- Deployed on Google Cloud Run
- 🔗 [Live demo](https://signals.flowpilot-ai.site/)

**[Expense Tracker MCP Server](https://github.com/thearyangupta/expense-tracker-mcp)**
A local MCP (Model Context Protocol) server exposing expense-management tools for MCP clients like Claude Desktop.
- Built with FastMCP, SQLAlchemy, and PostgreSQL

---

### 🛠️ Tech Stack

**GenAI/LLM:** LangGraph · LangChain · RAG pipelines · Hybrid Search (BM25 + Dense + RRF) · MCP · Gemini API · LLM Evaluation (RAGAS)
**ML/Data:** XGBoost · Logistic Regression · Isolation Forest · scikit-learn · pandas · leakage-safe feature engineering
**Backend:** FastAPI · PostgreSQL · pgvector · ChromaDB · SQLAlchemy · Pydantic · Firebase/Firestore
**Infra:** Redis · Celery · Docker · Google Cloud Run · AWS · GitHub Actions · Langfuse

---

### 📫 Reach me

[LinkedIn](https://linkedin.com/in/aryangupta-genai) · aryangwork@gmail.com
