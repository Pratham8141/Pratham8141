<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,100:00D9FF&height=120&section=header&animation=fadeIn" width="100%"/>

```
> initializing profile...
> loading modules: [systems] [infra] [realtime] [saas]
> all systems nominal.
```

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=36&duration=3000&pause=1000&color=FFFFFF&center=true&vCenter=true&width=800&lines=Pratham+Sharma)](https://git.io/typing-svg)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=400&size=15&duration=2500&pause=1200&color=00D9FF&center=true&vCenter=true&width=900&lines=Systems+Engineer+%E2%80%A2+SaaS+Builder+%E2%80%A2+Real-Time+Infrastructure;Distributed+systems+by+design%2C+not+by+accident.;Building+backends+that+hold+under+pressure.)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pratham8141)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://pratham8141.dev)
[![GitHub](https://img.shields.io/badge/GitHub-171515?style=flat-square&logo=github&logoColor=white)](https://github.com/Pratham8141)

<br/>

```
STATUS: ONLINE  |  BUILDING: ACTIVE  |  UPTIME: CONTINUOUS
```

</div>

---

> **`[MODULE: SYSTEM_PROFILE]`**

```yaml
name     : Pratham Sharma
status   : open to backend / systems engineering roles
focus    : event-driven architecture · real-time systems · SaaS infra
location : India
```

*I don't add scale later. I build for it the first time.*

---

> **`[MODULE: SYSTEM_METRICS]`**

```
  SYSTEMS DEPLOYED   →   5+        REAL-TIME FEATURES   →   8+
  APIs DESIGNED      →   10+       ASYNC PIPELINES      →   4+
  DB SCHEMAS OWNED   →   6+        INFRA COMPONENTS     →   12+
```

---

> **`[MODULE: DEPLOYED_SYSTEMS]`**

────────────────────────────────────────────────────────────

**`salez/`** — Multi-Tenant SaaS CRM
`STATUS: PRODUCTION` · `ISOLATION: SCHEMA-LEVEL`

Per-tenant isolation enforced at the schema level — not middleware. RBAC lives at the query layer. Notification pipeline fully async and decoupled from the request cycle. One deployment. Zero cross-tenant bleed.

```
Stack: React · Node.js · PostgreSQL (schema-per-tenant) · Redis · JWT · Docker
```

────────────────────────────────────────────────────────────

**`food-delivery-platform/`** — Fullstack Delivery System
`STATUS: PRODUCTION` · `SURFACES: 3`

Three clients, one backend contract. Order lifecycle runs through a server-side state machine — no client trust on transitions. RLS enforces access boundaries at the data layer. Staging and production never touch.

```
Stack: React Native (Expo) · Next.js · Supabase · PostgreSQL · RLS · Render · TypeScript
```

────────────────────────────────────────────────────────────

**`realtime-chat/`** — WebSocket Messaging Infrastructure
`STATUS: ACTIVE` · `TRANSPORT: PERSISTENT WS`

No polling. Presence and typing indicators via server-side event emission. Cursor-based pagination on history — no full-table scans. Reactions aggregated server-side with per-user indexing.

```
Stack: Node.js · WebSockets · PostgreSQL · Redis · React · Docker
```

────────────────────────────────────────────────────────────

**`pdf-toolkit/`** — Document Processing API
`STATUS: ACTIVE` · `PROCESSING: IN-MEMORY`

Stateless by design. Files stream in, process, and return — no disk writes, no shared state between requests. Heavy ops go to a background queue with retry semantics.

```
Stack: Python · FastAPI · PyMuPDF · Celery · Redis · Docker
```

────────────────────────────────────────────────────────────

**`synapse-ai/`** — LLM Application Frontend
`STATUS: EXPERIMENTAL` · `STREAM: SSE`

Token streaming via SSE. No reflow, no layout shift, no waiting. Context managed client-side with a lightweight token estimator. Target: sub-2s LCP, zero CLS on stream render.

```
Stack: Next.js · TypeScript · Tailwind CSS · SSE · OpenAI API · Vercel
```

────────────────────────────────────────────────────────────

---

> **`[MODULE: REQUEST_FLOW]`**

```
  CLIENT
    │
    ▼
  ┌─────────────────┐
  │   API Gateway   │  ← rate limiting · auth · request validation
  └────────┬────────┘
           │
     ┌─────┴──────┐
     ▼            ▼
 ┌────────┐  ┌──────────────┐
 │  REST  │  │  WebSocket   │  ← persistent · bi-directional
 └───┬────┘  └──────┬───────┘
     │               │
     ▼               ▼
  ┌──────────────────────────┐
  │     Service Layer        │  ← domain logic · state machines · RBAC
  └──────────┬───────────────┘
             │
     ┌───────┴────────┐
     ▼                ▼
 ┌──────────┐    ┌──────────┐
 │ Postgres │    │  Redis   │  ← cache · pub/sub · job queues
 └──────────┘    └──────────┘
             │
             ▼
  ┌──────────────────────┐
  │   Background Workers │  ← Celery · retry budgets · dead-letter
  └──────────────────────┘
```

---

> **`[MODULE: ARCHITECTURE]`**

```
Event-Driven Systems      async pipelines, durable by default — never blocking the request cycle
Real-Time Infrastructure  WS gateways, SSE streams, pub/sub at the transport layer
Distributed Systems       explicit consistency trade-offs — partition tolerance by design
Microservices             domain-bounded, independently deployed, contract-tested
Scalability               stateless compute · shared-nothing data · horizontal paths built in
```

*Incidents are expensive. Designing for failure is not.*

---

> **`[MODULE: LIVE_TRACE]`**

```log
[09:14:02] BOOT     loading tenant isolation middleware         ✓
[09:14:02] BOOT     registering websocket event handlers        ✓
[09:14:03] BOOT     connecting redis pub/sub channel            ✓
[09:14:03] BOOT     starting celery workers (concurrency=4)     ✓
[09:14:04] INFO     database pool initialized (max=20)
[09:14:04] INFO     JWT validation layer active
[09:14:05] WARN     p99 latency spike detected on /orders       → investigating
[09:14:06] INFO     dead-letter queue flushed — 3 jobs retried  ✓
[09:14:07] INFO     all systems nominal. accepting traffic.
```

---

> **`[MODULE: STACK_CONFIG]`**

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

**Data Layer**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)

**Infra & DevOps**

![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

**AI / LLM**

![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)

---

> **`[MODULE: GITHUB_STATS]`**

<div align="center">

<img height="175em" src="https://github-readme-stats.vercel.app/api?username=Pratham8141&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=00D9FF&icon_color=00D9FF&text_color=8B949E&include_all_commits=true&count_private=true"/>
<img height="175em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pratham8141&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=00D9FF&text_color=8B949E&langs_count=6"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=Pratham8141&theme=github-dark-blue&hide_border=true&background=0D1117&ring=00D9FF&fire=00D9FF&currStreakLabel=00D9FF&sideLabels=8B949E&dates=8B949E)](https://git.io/streak-stats)

</div>

---

> **`[MODULE: CONTRIBUTION_GRAPH]`**

<div align="center">
<img src="https://github.com/Pratham8141/Pratham8141/blob/output/github-contribution-grid-snake-dark.svg" alt="contribution graph" />
</div>

---

> **`[MODULE: CORE_PRINCIPLES]`**

```
01.  systems fail          →  design for it before writing a single line
02.  latency is a feature  →  p99 matters as much as p50
03.  scale is planned      →  not added after the incident
04.  trust no client       →  auth and validation live at the server. always.
05.  async by default      →  decouple what doesn't need to be coupled
06.  idempotency first     →  retries happen. build for them.
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00D9FF,100:0D1117&height=80&section=footer&reversal=true" width="100%"/>

```
> session terminated.
> systems running. stack holding. building continues.
```

</div>
