## Hi, I'm Namiq — AI Engineer

**I build AI systems that hold up in front of real users, and I measure them.**

Most AI demos break the moment a chatbot invents a refund policy or a wrong
deadline. My work focuses on the part that matters in production: agents that
**prove every claim against source documents**, **fail over between providers**,
**remember users across sessions**, and **escalate to a human** when they should.
I ship and run the systems myself, and I publish the evaluations, including the
results that did not work.

🟢 **Open to AI Engineer / LLM Engineer roles and freelance projects** — remote or on-site.
📫 [namiq.sarxanli@gmail.com](mailto:namiq.sarxanli@gmail.com) ·
[LinkedIn](https://www.linkedin.com/in/namiq-sarxanl%C4%B1-706546149/)

---

### What I can build for your team

| Need | What I deliver |
|---|---|
| **Customer-facing AI support** | Agents whose replies are checked by code against your policies before sending, so they cannot make hallucinated promises |
| **Measured RAG and legal/document research** | Retrieval with citations to the exact source, verbatim-quote checks, and pre-registered evaluations |
| **Multi-agent automation** | Orchestrated agent teams (planner → workers → critic) with live progress tracking |
| **Voice agents** | Real-time phone and voice assistants (Twilio, OpenAI Realtime) connected to CRM data |
| **Production web platforms** | Phone-first apps with audited data, offline fallbacks, backups and monitoring, run through a live event |
| **Business workflow automation** | n8n pipelines with human approval steps, scraping, OCR and Telegram/Gmail/Sheets integrations |

---

### Featured work

**[AI Summit](https://github.com/namiqsarxanli-creator/ai-summit): an event platform run in production**
Networking and gamification for an AI Summit in Baku, used on 13 Nov 2026 by **314 registered attendees**.
- QR contact cards, booth and door scanning with an offline queue, a live leaderboard and venue screens
- An **append-only points ledger**: every award is deduplicated, every correction is a new entry, every staff action is audited
- Ran the system on the day. All 250 health checks passed, and the pre-event load test with 500 virtual users had 0 errors
- An honest [event-day post-mortem](https://github.com/namiqsarxanli-creator/ai-summit/blob/main/docs/postmortem-2026-11-13.md) covering what went wrong and how it was fixed live without losing data
- FastAPI · PostgreSQL · Next.js · `mypy --strict` · 180+ test files

**[Mizan](https://github.com/namiqsarxanli-creator/Mizan): measured legal research for Azerbaijani labour law**
- Answers cite the exact article **in force on a given date** (temporal RAG). A Neo4j citation graph also brings in Constitutional Court decisions
- Retrieval Recall@5 **0.946**. The prompt-injection screen blocks **98.2%** of held-out attacks with 0 of 281 benign questions blocked
- A local LoRA verifier reaches **98.4%** of the API model's F1 at **7.3× lower cost**
- Negative results are reported too: multi-agent was worse than single-shot, and the fine-tuned embedder missed its gate
- Evaluation sets published on Hugging Face as **AzLegalBench**

**[Probo](https://github.com/namiqsarxanli-creator/probo): AI agency with zero tolerance for invented promises**
Inspired by *Moffatt v. Air Canada* (2024), where an airline paid for its chatbot's made-up refund policy.
- Every sentence sent to a customer must quote the company's rules verbatim. A **deterministic code verifier**
  (not another LLM) blocks invented numbers, dates, and prohibitions flipped into permissions
- AI "employees" are hired via exams and fired when the **95% Wilson lower bound** of their error rate crosses the threshold
- Random **human audits** measure what the verifier can't catch, reported as confidence intervals

**[The Aigency](https://github.com/namiqsarxanli-creator/the-aigency): a creative agency run by AI agents**
- A text brief spawns CEO, Strategist, Copywriter, Designer, Developer and QA agents, tracked on a live WebSocket Kanban
- A critic agent gates every output through a revision loop, and **3-provider LLM failover** retries automatically
- A Twilio + OpenAI Realtime **voice sales agent** uses CRM data as context. **244 tests**, fully network-mocked

**More projects**

| Project | Highlights |
|---|---|
| [AkademIQ](https://github.com/namiqsarxanli-creator/AkademIQ) | Multi-tenant ERP for education centres: config-driven modules, role permissions, finance and payroll, encrypted backups, 2FA |
| [AIWorks Summit Playground](https://github.com/namiqsarxanli-creator/aiworks-summit-playground) | Conference booth game: MediaPipe face and pose scoring in the browser, vision-model judging with a racing fallback chain, live TV mirror |
| [Tralala](https://github.com/namiqsarxanli-creator/tralala) | Live quiz for a room of colleagues: QR join, eight question types, an AI explainer (Groq with Claude fallback) |
| [Admissions QLoRA + RAG](https://github.com/namiqsarxanli-creator/azerbaijani-admissions-qlora-rag) | Azerbaijani admissions chatbot experiment: NF4 QLoRA, E5/FAISS retrieval, raw-output evaluation |
| [VISION](https://github.com/namiqsarxanli-creator/vision-voice-assistant) | Clap-to-wake voice assistant with hand-gesture control, Groq/OpenAI fallback and Gmail/Calendar/Sheets tools |
| [MemoryDesk](https://github.com/namiqsarxanli-creator/MemoryDesk) | Layered agent memory on Cloudflare Workers + D1, compared side by side with a "memory off" mode |
| [Forex Signal Desk](https://github.com/namiqsarxanli-creator/forex-signal-desk) | News scoring in n8n → human approval → FastAPI risk limits → MT5 execution |
| [Real-Estate Deal Finder](https://github.com/namiqsarxanli-creator/real-estate-deal-finder) | Listing scraping and OCR, market-price estimation, below-market alerts to Telegram |
| [El Regreso](https://github.com/namiqsarxanli-creator/el-regreso) | LangGraph stateful graph with checkpointing, live graph visualization |

---

### Tech stack

**AI / LLM:** Anthropic Claude · OpenAI · Groq · Gemini · OpenRouter · LangGraph · Realtime voice · Tool calling · LLM evaluation
**Retrieval & ML:** RAG · Qdrant · Neo4j · FAISS · bge-m3 / E5 embeddings · LoRA / QLoRA · MediaPipe
**Backend:** Python · FastAPI · SQLAlchemy · PostgreSQL · Alembic · WebSockets / SSE · pytest · mypy
**Frontend / Edge:** TypeScript · Next.js · React · Vitest · Cloudflare Workers / D1
**Ops & Integrations:** Docker · Caddy · DigitalOcean · backups & monitoring · n8n · Twilio · Telegram · Google Workspace APIs
