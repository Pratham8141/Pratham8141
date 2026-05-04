<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=28&duration=3000&pause=1000&color=00D9FF&center=true&vCenter=true&width=700&lines=Hey%2C+I'm+Arjun+Singh.;Backend+%26+Systems+Engineer.;I+build+systems+that+scale.;Distributed+systems+%E2%80%94+done+right.)](https://git.io/typing-svg)

<br/>

```
Backend & Systems Engineer  ·  Distributed Systems  ·  SaaS  ·  AI Infrastructure
```

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/yourprofile)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://yourwebsite.dev)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:you@email.com)

</div>

---

## About

I design and ship production-grade backend systems — not side projects, not tutorials. I work across the full lifecycle of SaaS products: API design, event-driven pipelines, real-time systems, and AI integrations that run at scale.

My focus is on correctness, performance, and architecture that doesn't collapse under load. I've built CRMs, real-time communication platforms, and LLM tooling from scratch — making deliberate choices around consistency, fault tolerance, and operational simplicity at every layer.

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-14354C?style=flat-square&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)

**Backend & Systems**

![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=google&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)

**AI / LLM**

![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square&logo=pinecone&logoColor=white)

---

## Selected Work

<table>
<tr>
<td width="50%" valign="top">

### NexusCRM
**Multi-tenant SaaS CRM with sub-100ms query response at scale.**

Built a fully isolated multi-tenant architecture with per-tenant schema partitioning in PostgreSQL, RBAC, webhook engine, and a real-time activity feed powered by Kafka. Handles 50K+ records per tenant without degradation.

`Python` `FastAPI` `PostgreSQL` `Kafka` `Redis` `Docker`

</td>
<td width="50%" valign="top">

### StreamLine — Real-Time Chat Platform
**Production-ready messaging infrastructure with presence, rooms, and delivery guarantees.**

Engineered a WebSocket gateway with horizontal scaling via Redis pub/sub. Message persistence with ordered delivery semantics, reconnect handling, and read receipts — all under 30ms round-trip in local benchmarks.

`Go` `WebSockets` `Redis` `PostgreSQL` `Kubernetes`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ContextCore — RAG API Platform
**Drop-in retrieval-augmented generation backend for product teams.**

REST API layer over a vector store pipeline — handles document ingestion, chunking, embedding, and retrieval with re-ranking. Built to be model-agnostic with support for OpenAI, Anthropic, and local models via HuggingFace.

`Python` `FastAPI` `Pinecone` `LangChain` `OpenAI` `PostgreSQL`

</td>
<td width="50%" valign="top">

### Dispatch — Job Queue Engine
**Reliable background job processing with retry semantics and observability.**

Custom job queue implementation on top of RabbitMQ with priority lanes, dead-letter queues, exponential backoff, and a lightweight web dashboard. Used in production to power scheduled reports and async workflows.

`TypeScript` `Node.js` `RabbitMQ` `Redis` `PostgreSQL`

</td>
</tr>
</table>

---

## Engineering Philosophy

```
Systems I build are designed around four constraints:

  → Fault isolation     — failures are local, never cascading
  → Horizontal scale    — stateless services, shared-nothing where possible
  → Operational clarity — observable, debuggable, and boring to operate
  → Correctness first   — eventual consistency only where it's a deliberate trade-off
```

I default to **event-driven architecture** for anything async — Kafka for durability, Redis for speed. For service boundaries, I follow **domain-driven decomposition**: services own their data, communicate via contracts, and deploy independently.

Distributed systems are hard. I've debugged clock skew in distributed locks, traced message ordering failures across partitioned Kafka topics, and rebuilt auth flows that looked fine until load hit. That experience shapes every design decision.

---

## GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=00D9FF&icon_color=00D9FF&text_color=C9D1D9&include_all_commits=true&count_private=true"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yourusername&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=00D9FF&text_color=C9D1D9&langs_count=6"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=yourusername&theme=github-dark-blue&hide_border=true&background=0D1117&ring=00D9FF&fire=00D9FF&currStreakLabel=00D9FF)](https://git.io/streak-stats)

</div>

---

## Contribution Graph

<div align="center">

[![Snake animation](https://raw.githubusercontent.com/yourusername/yourusername/output/github-contribution-grid-snake-dark.svg)](https://github.com/yourusername)

</div>

> **Note:** To enable the snake animation, add this GitHub Action to your profile repo at `.github/workflows/snake.yml`:
>
> ```yaml
> name: Generate Snake
> on:
>   schedule:
>     - cron: "0 0 * * *"
>   workflow_dispatch:
> jobs:
>   generate:
>     runs-on: ubuntu-latest
>     steps:
>       - uses: Platane/snk@v3
>         with:
>           github_user_login: ${{ github.repository_owner }}
>           outputs: |
>             dist/github-contribution-grid-snake.svg
>             dist/github-contribution-grid-snake-dark.svg?palette=github-dark
>       - uses: crazy-max/ghaction-github-pages@v3
>         with:
>           target_branch: output
>           build_dir: dist
>         env:
>           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
> ```

---

<div align="center">

```
Building systems that scale.
```

</div>
