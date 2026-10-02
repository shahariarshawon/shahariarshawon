<img width="1584" height="396" alt="Al Shahariar Arafat Shawon — Backend Engineer" src="https://github.com/user-attachments/assets/55a654a5-8aad-438e-8a06-382541a2eb88" />

<h1 align="center">Al Shahariar Arafat Shawon</h1>

<p align="center">
  <b>Backend Engineer · Multi-Tenant SaaS · AI Infrastructure</b><br/>
  TypeScript · Node.js · NestJS · PostgreSQL · Redis · Kafka · Docker
</p>

<p align="center">
  <a href="https://shahariararafat.vercel.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"/></a>
  <a href="https://www.linkedin.com/in/alshahariardev"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:shahariarshawon.dev@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://www.youtube.com/@learnwithshahariar"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube"/></a>
</p>

<p align="center"><i>📍 Dhaka, Bangladesh · 🌍 Open to remote backend roles with international teams</i></p>

---

## About Me

I build the server side of SaaS products: APIs, access control, data models, and the infrastructure that keeps multi-tenant systems **isolated, auditable, and cost-controlled**.

- 💼 **Backend Developer & Technical Instructor** at **Rise Together BD** (remote), building production services with NestJS, PostgreSQL, Redis, and Docker
- 🧠 Building **Tollbooth AI**, a multi-tenant LLM gateway that governs how applications access AI providers
- 🎓 B.Sc. in Computer Science & Engineering at **IUBAT** (expected 2028)
- 🧩 Competitive programmer on **Codeforces** and **LeetCode**
- 🎙️ Teach backend engineering in plain language on **[Learn With Shahariar](https://www.youtube.com/@learnwithshahariar)**

---

## Featured Projects

### 🛡️ Tollbooth AI — Multi-Tenant LLM Gateway & AI Governance Platform
<!-- Replace TOLLBOOTH_REPO_URL and TOLLBOOTH_LIVE_URL with real links, or delete them -->
[Repository](TOLLBOOTH_REPO_URL) · [Live Demo](TOLLBOOTH_LIVE_URL)

A gateway that sits between applications and AI providers to control **access, cost, and reliability** of AI usage.

- Per-tenant **API key management, RBAC, and rate limiting** on every request
- **Budget enforcement** applied *before* a request reaches a model, with token and cost tracking per tenant
- **Provider routing** across AI providers through a single gateway
- **Event-driven usage processing**: usage events flow through Kafka into PostgreSQL for analytics and audit logging

```mermaid
flowchart LR
    A[Client Apps] -->|API key| G[Gateway<br/>NestJS]
    G --> C{Auth · RBAC<br/>Rate limit · Budget}
    C -->|allowed| R[Provider Router]
    R --> P1[AI Provider A]
    R --> P2[AI Provider B]
    G <--> AI[AI Service<br/>FastAPI]
    G <--> RD[(Redis)]
    G -->|usage events| K[[Kafka]]
    K --> DB[(PostgreSQL<br/>usage · costs · audit)]
```

`NestJS` `TypeScript` `FastAPI` `PostgreSQL` `Prisma` `Redis` `Kafka` `pgVector` `Docker`

---

### 🧾 Rise Together — Recruitment Automation Platform
<!-- Replace RECRUITMENT_LIVE_URL with a real link, or delete it -->
[Live](RECRUITMENT_LIVE_URL)

A recruitment workflow platform built for Rise Together BD, covering the hiring lifecycle from job publishing to the final decision.

- **Stage-driven pipeline**: resume processing, eligibility checks, and candidate scoring advance applicants automatically
- Project submission and evaluation, interview scheduling, and hiring decisions in one workflow
- Automated **email notifications and status updates** at every stage
- Containerized deployment on a Linux VPS

`NestJS` `TypeScript` `PostgreSQL` `Redis` `Docker` `Linux VPS`

---

### 🛒 SureSale — Multi-Vendor Marketplace Platform
<!-- Replace SURESALE_REPO_URL and SURESALE_LIVE_URL with real links, or delete them -->
[Repository](SURESALE_REPO_URL) · [Live](SURESALE_LIVE_URL)

Led backend development for a marketplace where vendors, buyers, and admins share one platform under separate role permissions.

- **Multi-role RBAC**, vendor onboarding, and product management
- Tiered **subscription system** for vendors
- Real-time **messaging and notifications**
- Redis caching for high-read paths and Dockerized deployment

`Node.js` `Express.js` `TypeScript` `PostgreSQL` `Redis` `Docker`

---

## Tech Stack

**Backend**<br/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
<img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white"/>
<img src="https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socketdotio&logoColor=white"/>

**Data & Messaging**<br/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white"/>

**AI Engineering**<br/>
<img src="https://img.shields.io/badge/LLM%20Gateways-111111?style=flat-square"/>
<img src="https://img.shields.io/badge/RAG-111111?style=flat-square"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/Vector%20Search-111111?style=flat-square"/>

**DevOps & Tooling**<br/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
<img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white"/>
<img src="https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white"/>
<img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black"/>
<img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white"/>
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>

<sub>Also comfortable with: React, Next.js, Tailwind CSS · C++ for competitive programming</sub>

---

## How I Approach Backend Work

- **Design for tenants from day one.** Isolation, per-tenant limits, and attribution are much harder to add later.
- **Keep the request path lean.** Metering, analytics, and notifications belong in events, not in the user's wait time.
- **Make systems auditable.** If money or access is involved, every decision should leave a record.
- **Ship it, don't just build it.** Docker, Linux, and CI/CD are part of the job, not someone else's problem.

---

## Achievements

- 🚀 **NASA Space Apps Challenge 2026** — Participant
- 🛠️ **The Infinity AI BuildFest 2026** — Participant
- 🏁 **3× Software Hackathon** Participant
- 🧩 **Competitive Programming** — Codeforces & LeetCode

---

## Currently Exploring

Distributed systems design · Observability for event-driven services · Go for high-performance backend services

---

## Let's Connect

I'm open to **remote Backend Engineer roles** with international teams, especially in SaaS, platform, and AI infrastructure.<br/>
The fastest way to reach me is **[shahariarshawon.dev@gmail.com](mailto:shahariarshawon.dev@gmail.com)** or **[LinkedIn](https://www.linkedin.com/in/alshahariar-dev)**.

<p>
  <a href="https://stackoverflow.com/users/31131673/al-shahariar-arafat-shawon"><img src="https://img.shields.io/badge/Stack%20Overflow-F58025?style=flat-square&logo=stackoverflow&logoColor=white" alt="Stack Overflow"/></a>
  <a href="https://medium.com/@shahariarshawon.dev"><img src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white" alt="Medium"/></a>
  <a href="https://shahariararafat.vercel.app"><img src="https://img.shields.io/badge/Learn%20With%20Shahariar-111111?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio"/></a>
</p>

<!-- Optional: one stats card. The public instance is sometimes rate-limited; remove it if it shows an error.
<img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shahariarshawon&layout=compact&hide_border=true" />
-->

> *Build deeply. Learn publicly. Teach simply.*
