<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,100:00D9FF&height=120&section=header&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=36&duration=3000&pause=1000&color=FFFFFF&center=true&vCenter=true&width=800&lines=Pratham+Sharma)](https://git.io/typing-svg)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=400&size=15&duration=2500&pause=1200&color=00D9FF&center=true&vCenter=true&width=900&lines=Systems+Engineer+%E2%80%A2+SaaS+Builder+%E2%80%A2+Real-Time+Infrastructure;Distributed+systems+by+design%2C+not+by+accident.;Building+backends+that+hold+under+pressure.)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pratham8141)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://pratham8141.dev)
[![GitHub](https://img.shields.io/badge/GitHub-171515?style=flat-square&logo=github&logoColor=white)](https://github.com/Pratham8141)

</div>

---

## `> system.profile`

```yaml
name        : Pratham Sharma
status      : Building in public — open to backend / systems engineering roles
focus       : Event-driven architecture · Real-time systems · SaaS infrastructure
stack       : React · Node.js · Python · PostgreSQL · Redis · WebSockets · Docker
location    : India
```

---

## `> ls -la deployed/`

### `salez/` — Multi-Tenant SaaS CRM

> Full-stack CRM with isolated tenant workspaces, role-based access control, and live activity feeds.

Per-tenant data isolation enforced at the schema level in PostgreSQL. RBAC is evaluated at the query layer — not just middleware. The notification pipeline runs asynchronously, decoupled from the request cycle. Built to support multiple organizations under a single deployment without cross-tenant data bleed.

```
Stack: React · Node.js · PostgreSQL (schema-per-tenant) · Redis · JWT · Docker
```

---

### `food-delivery-platform/` — Fullstack Delivery System

> End-to-end food ordering system spanning mobile, web admin, and a real-time order state engine.

Three client surfaces, one backend contract: a React Native (Expo) app for customers, a Next.js operator dashboard for restaurants, and Supabase handling data persistence with row-level security enforcing access boundaries. Order lifecycle managed via server-side state machine — no client trust on transitions. Deployed on Render with staging and production isolation.

```
Stack: React Native (Expo) · Next.js · Supabase · PostgreSQL · RLS · Render · TypeScript
```

---

### `realtime-chat/` — WebSocket Messaging Infrastructure

> Production-grade chat system with presence tracking, message reactions, typing indicators, and paginated history.

Persistent WebSocket connections handle bi-directional message delivery with acknowledgment semantics. Typing indicators and online presence are managed via server-side event emission — no polling. Message history is paginated with cursor-based navigation to avoid full-table scans. Reactions stored as aggregated counts with per-user indexing.

```
Stack: Node.js · WebSockets · PostgreSQL · Redis · React · Docker
```

---

### `pdf-toolkit/` — Document Processing API

> REST API for PDF operations — merge, split, compress, extract text, watermark, and camera capture ingestion.

Stateless service architecture: files stream in, are processed in-memory, and return directly — no persistent file storage, no side effects between requests. Camera capture flow converts mobile image input to PDF via server-side preprocessing. Heavy batch operations dispatched to a background worker queue with retry semantics.

```
Stack: Python · FastAPI · PyMuPDF · Celery · Redis · Docker
```

---

### `synapse-ai/` — LLM Application Frontend

> Minimal, fast interface for interacting with large language models — built around streaming and low-latency UX.

Token streaming rendered in real-time via Server-Sent Events — responses appear character by character with no reflow or layout shift. Context window managed client-side using a lightweight token estimator. Conversation history serialized per-session. Performance targets: sub-2s LCP, zero CLS on stream render.

```
Stack: Next.js · TypeScript · Tailwind CSS · SSE · OpenAI API · Vercel
```

---

## `> cat engineering.focus`

```
Domain                    Approach
──────────────────────    ─────────────────────────────────────────────────────────
Event-Driven Systems      Async pipelines decoupled from the request cycle — durable by default
Real-Time Infrastructure  WebSocket gateways, SSE streams, and pub/sub at the transport layer
Distributed Systems       Explicit consistency trade-offs — partition tolerance by design
Microservices             Domain-bounded services, independent deployments, contract-tested APIs
Scalability               Stateless compute, shared-nothing data, horizontal scale paths built in
```

Failure modes are designed before features ship. Idempotency, dead-letter queues, and retry budgets are first-class architecture concerns — not patches applied after incidents.

---

## `> cat stack.config`

**Languages**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-14354C?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Backend & Systems**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![REST](https://img.shields.io/badge/REST_API-FF6C37?style=flat-square&logo=postman&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)

**Cloud & DevOps**

![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)

**AI / LLM**

![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

---

## `> github --stats`

<div align="center">

<img height="175em" src="https://github-readme-stats.vercel.app/api?username=Pratham8141&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=00D9FF&icon_color=00D9FF&text_color=8B949E&include_all_commits=true&count_private=true"/>
<img height="175em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pratham8141&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=00D9FF&text_color=8B949E&langs_count=6"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=Pratham8141&theme=github-dark-blue&hide_border=true&background=0D1117&ring=00D9FF&fire=00D9FF&currStreakLabel=00D9FF&sideLabels=8B949E&dates=8B949E)](https://git.io/streak-stats)

</div>

---

## `> git log --graph`

<div align="center">

<img src="https://github.com/Pratham8141/Pratham8141/blob/output/github-contribution-grid-snake-dark.svg" alt="contribution graph" />

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00D9FF,100:0D1117&height=80&section=footer&reversal=true" width="100%"/>

```
Building systems that scale.
```

</div>
