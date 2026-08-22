# Hi, I'm Aryan Gupta 👋

Applied AI Engineer building production-ready RAG systems, LLM agents, and backend infrastructure with Python, FastAPI, and LangGraph.

I don't just prototype — I ship. Both projects below are live, deployed, and evaluated with real metrics.

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

**[Expense Tracker MCP Server](https://github.com/thearyangupta/expense-tracker-mcp)**
A local MCP (Model Context Protocol) server exposing expense-management tools for MCP clients like Claude Desktop.
- Built with FastMCP, SQLAlchemy, and PostgreSQL

---

### 🛠️ Tech Stack

**GenAI/LLM:** LangGraph · LangChain · RAG pipelines · Hybrid Search (BM25 + Dense + RRF) · MCP · LLM Evaluation (RAGAS)
**Backend:** FastAPI · PostgreSQL · pgvector · ChromaDB · SQLAlchemy · Pydantic
**Infra:** Redis · Celery · Docker · Google Cloud Run · AWS · GitHub Actions · Langfuse

---

### 📫 Reach me

[LinkedIn](https://linkedin.com/in/aryan-gupta-ba042b253) · aryangwork@gmail.com
