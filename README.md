## Hi, I'm Arpit 👋

I build products end to end: the frontend, the backend, the infrastructure, and everything in between. Give me a problem and I'll own it from the first commit to production and keep it running after that.

- 🧩 **I'll work on any problem.** Distributed systems, realtime UI, Office.js, search, billing, and deployment are all part of the job.
- 🛠️ **I care about building products.** I want them to be useful, reliable, and good to use.
- 🚀 **I take ownership from zero to shipped.** That means design, code, tests, deploys, observability, and support.
- 🤖 **I'm AI-forward.** I build AI products, I use AI coding agents every day, and I follow everything happening in the field.

📍 Melbourne, Australia

---

### 📊 Where my commits are

Most of my work happens in private company repositories on Azure DevOps, so it doesn't show up on GitHub by default.

<p>
  <img src="https://img.shields.io/badge/3,290+_commits-since_Nov_2024-7c3aed?style=for-the-badge" alt="3,290+ commits since Nov 2024" />
  <img src="https://img.shields.io/badge/14_private_repos-mostly_solo-6d28d9?style=for-the-badge" alt="14 private repos, mostly solo" />
  <img src="https://img.shields.io/badge/366_days-with_commits-5b21b6?style=for-the-badge" alt="366 days with commits" />
</p>

My contribution graph includes that activity. Each work commit appears as an empty commit with the same timestamp in a private mirror repo. No code, commit messages, or repository names leave the company repos.

---

### 🏗️ What I've built at work

**Curiosity: a multi-client AI agent platform.** I'm the sole engineer.
One agent runtime serves a web chat app and native **Word, Excel, PowerPoint, and Outlook** add-ins. It's about 70K lines of TypeScript with about 700 tests.

- **Agent runtime**
  - Each run is executed by a single worker that holds a lease on it.
  - Work is dispatched from self-hosted **Convex** into **BullMQ/Redis** queues and executed by **Bun** workers.
  - Output streams over SSE backed by **Redis Streams**, and clients can resume after a disconnect.
  - Runs can be cancelled cleanly.
  - The queue protocol is versioned.
- **Safe edits to Office documents**
  - The model's tools run inside the user's Office document.
  - Tool calls are claimed under leases.
  - Results are recorded in a journal, and a write interrupted mid-flight is never repeated.
  - The user approves destructive actions.
- **20 Office.js tools**, including:
  - Word reports generated as raw OOXML.
  - About 85 Excel actions, including pivot tables and conditional formatting.
  - PowerPoint slides the model renders and inspects to correct its own designs.
- **Context and memory**
  - Prompt caching and token budgeting.
  - Structured compaction of long conversations.
  - Long-term memory with hybrid keyword and vector search, plus version history.
  - Rolling summaries of past chats.
- **Skills and tools**
  - A versioned skills system, with an LLM that decides when a skill is relevant.
  - MCP integrations, including an Elasticsearch MCP server for company documents with index allowlists.
  - Document retrieval over attachments, image generation, and handing tasks between agents.
- **Platform**
  - Entra ID auth, checked at the API and again at the database layer.
  - A credit ledger in integer micro-USD that stays correct when operations repeat.
  - OpenTelemetry tracing, eval harnesses for the agent, and Azure deployment with Docker, Envoy, Container Apps, and Static Web Apps.

**Einstein: an internal knowledge and analytics platform**
- **Frontend:** React 19, about 83K lines. It includes the Curiosity chat UI with resumable streaming and a live view of the agent's tool calls, cost and duration benchmarking with D3 regression and Gantt charts, a How-To guide library, maps, and admin tooling.
- **Backend:** Express, MongoDB, Postgres, and Elasticsearch, with about 100 endpoints. It includes enterprise search across SharePoint and regional file shares, filtered by each user's document permissions.

**Also shipped:** an assessment platform (frontend and backend), an AI bill-extraction pipeline with SharePoint and Entra sync, a visitor portal, a CMS-backed hub, and the Envoy relay in front of the stack.

---

### 🧰 Tools I use

**AI:** Vercel AI SDK · OpenAI / Azure OpenAI · MCP · agents & tool calling · RAG · evals · AI coding agents

**Frontend:** TypeScript · React · Vite · Tailwind · TipTap · D3 · Office.js

**Backend:** Bun · Hono · Express · Convex · Redis / BullMQ · MongoDB · PostgreSQL · Elasticsearch

**Infra:** Azure (Container Apps, Static Web Apps, Blob, Entra ID, App Insights) · Docker · Envoy · Nginx · OpenTelemetry · Azure Pipelines

---

### 🔗 Connect

<p>
  <a href="https://arpitsingh.dev"><img src="https://img.shields.io/badge/Portfolio-7c3aed?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/arpitsingh-jkirito/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://twitter.com/Arpit_JKirito"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>
  <a href="mailto:byrxarpitsingh@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>
