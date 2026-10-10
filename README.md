## Hi, I'm Namiq — AI Engineer

**I build LLM agents that businesses can actually trust in front of customers.**

Most AI demos break the moment a chatbot invents a refund policy or a wrong
deadline. My work focuses on the part that matters in production: agents that
**prove every claim against source documents**, **fail over between providers**,
**remember users across sessions**, and **escalate to a human** when they should.

🟢 **Open to AI Engineer / LLM Engineer roles and freelance projects** — remote or on-site.
📫 [namiq.sarxanli@gmail.com](mailto:namiq.sarxanli@gmail.com) ·
[LinkedIn](https://www.linkedin.com/in/namiq-sarxanl%C4%B1-706546149/)

---

### What I can build for your team

| Need | What I deliver |
|---|---|
| **Customer-facing AI support** | Agents whose replies are checked by code against your policies before sending — no hallucinated promises |
| **Multi-agent automation** | Orchestrated agent teams (planner → workers → critic) with live progress tracking |
| **Voice agents** | Real-time phone/voice assistants (Twilio, OpenAI Realtime) connected to CRM data |
| **AI memory & personalization** | Short/long-term, semantic/episodic memory that survives sessions |
| **Business workflow automation** | n8n pipelines with human approval steps, scraping, OCR, Telegram/Gmail/Sheets integrations |

---

### Featured work

**[Probo](https://github.com/namiqsarxanli-creator/probo) — AI agency with zero tolerance for invented promises**
Inspired by *Moffatt v. Air Canada* (2024), where an airline paid for its chatbot's made-up refund policy.
- Every sentence sent to a customer must quote the company's rules verbatim; a **deterministic code
  verifier** (not another LLM) blocks invented numbers, dates, and prohibitions flipped into permissions
- AI "employees" are hired via paid exams (75% pass bar), paid by real token prices, and fired only when
  the **95% Wilson lower bound** of their error rate crosses the threshold
- Random **human audits** measure what the verifier can't catch, reported as honest confidence intervals
- Budget guardrails: cost-cutting at 80% spend, hard stop at 100%

**[The Aigency](https://github.com/namiqsarxanli-creator/the-aigency) — a creative agency run by AI agents**
- A text brief spawns CEO, Strategist, Copywriter, Designer, Developer & QA agents, tracked on a live WebSocket Kanban
- Critic agent gates every output through a revise loop
- **3-provider LLM failover** (Groq → Gemini → Hugging Face) with automatic retry
- Twilio + OpenAI Realtime **voice sales agent** with CRM-driven context
- **244 tests**, fully network-mocked

**More projects**

| Project | Highlights |
|---|---|
| [VISION](https://github.com/namiqsarxanli-creator/vision-voice-assistant) | Clap-to-wake voice assistant, hand-gesture control, Groq/OpenAI fallback, Gmail/Calendar/Sheets tools |
| [MemoryDesk](https://github.com/namiqsarxanli-creator/MemoryDesk) | Layered agent memory on Cloudflare Workers + D1, side-by-side "memory off" comparison |
| [Forex Signal Desk](https://github.com/namiqsarxanli-creator/forex-signal-desk) | News scoring in n8n → human approval → FastAPI risk limits → MT5 execution |
| [Real-Estate Deal Finder](https://github.com/namiqsarxanli-creator/real-estate-deal-finder) | Listing scraping + OCR, market-price estimation, below-market alerts to Telegram |
| [El Regreso](https://github.com/namiqsarxanli-creator/el-regreso) | LangGraph course project I designed: stateful graphs & checkpointing, with starter, solution and rubric |

---

### Tech stack

**AI / LLM:** OpenAI · Groq · Gemini · LangGraph · Realtime voice · Prompt & tool design · LLM evaluation
**Backend:** Python · FastAPI · SQLAlchemy · WebSockets · pytest
**Frontend / Edge:** TypeScript · Next.js · React · Cloudflare Workers / D1
**Automation & Integrations:** n8n · Twilio · Telegram · Google Workspace APIs · Docker

---

*I also teach AI engineering — designing hands-on lessons on LangGraph and agent memory.*
