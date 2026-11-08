# Hi, I'm William Macarini

**Senior Software Engineer** — distributed systems, cloud-native architecture, and high-scale backend platforms in **Go** and **.NET**.

Currently at **Mercado Pago / Mercado Libre**, building and evolving fiscal and billing systems that process millions of requests daily across Latin America.

---

## What I work on

- **Fiscal & billing platforms at scale** — systems serving 80K+ sellers across Brazil, Chile, and Peru
- **Event-driven Go services** — microservices, Kafka, Redis Streams, CQRS
- **Payment & fintech domain** — LatAm payment rails (Pix, boleto), idempotency, reconciliation, tax rules
- **Hard performance problems** — query optimization, throughput, observability, reliability

---

## Featured projects

### 🎂 Confeito Gestão — multi-tenant SaaS for bakery management

Full product built end-to-end: multi-tenant SaaS with per-tenant data isolation, technical costing sheets that propagate ingredient price changes through recipes via Redis Streams, integrated online store, and order workflow (quote → production → delivery).

| | |
|---|---|
| **Backend** | Go 1.25, Fiber, GORM, PostgreSQL 16, Redis |
| **Frontend** | Next.js 15, TypeScript, Tailwind, shadcn/ui |
| **Auth** | JWT with refresh tokens, rate limiting, tenant middleware |
| **Quality** | 99 test files (Go + TS), Docker Compose, Postman collection |
| **Scale** | ~62K LOC across two apps + shared types package |

> Private repository (commercial product). The architecture is documented publicly — see below.

### 🏗️ confeito-architecture — design decisions behind the SaaS

Architecture write-ups extracted from the production codebase above. Not tutorials — the actual decisions, their trade-offs, and what I'd do differently.

- **Cost cascading via Redis Streams** — how an ingredient price change propagates through preparations, recipes and catalog products, including the `XAUTOCLAIM` / PEL failure mode that only surfaces when a worker dies mid-message in production.
- **Multi-tenancy** — shared tables with a single enforcement choke point, its honest weaknesses, and the documented trigger that would make me revisit the decision.
- **Testing strategy** — 43 test files across services, handlers and middleware.

🔗 [github.com/williammacarini/confeito-architecture](https://github.com/williammacarini/confeito-architecture)

### 🧱 solid-principles — SOLID in C#, violation and fix

Five principles, each shown twice: the code that violates it and the refactor that fixes it. Drawn from payments and billing rather than the usual shapes and animals — so the trade-offs are real, and a couple of the refactors are only worth doing once the second case appears.

**10 tests passing**, .NET 10, zero build warnings.

🔗 [github.com/williammacarini/solid-principles](https://github.com/williammacarini/solid-principles)

### 🧪 DotNetLab — independent .NET labs

Personal lab of self-contained .NET experiments: Saga Pattern with MassTransit state machine, four rate-limiting algorithms (Fixed Window, Sliding Window, Token Bucket, Leaky Bucket), each with its own solution, tests, and Makefile targets.

🔗 [github.com/williammacarini/DotNetLab](https://github.com/williammacarini/DotNetLab)

### ✍️ williammacarini.com.br — bilingual engineering blog

**21 articles, each published in Portuguese and English** — on Go patterns, .NET, architecture, and AI-assisted software engineering. Written in MDX with a custom Next.js App Router setup.

🔗 [williammacarini.com.br](https://www.williammacarini.com.br)

Selected writing:

- Chain of Responsibility in Go
- Functional Options in Go
- Saga Pattern in Go
- Observer Pattern in Go
- Pipeline Pattern in Go
- Go 1.26 Green Tea GC
- SOLID Principles in C#
- Builder Pattern in C#
- AI-assisted SDLC orchestration
- Claude Code hooks & skills

---

## Tech stack

**Languages** — Go · C# · TypeScript · Python · F#

**Backend** — Fiber · ASP.NET Core · GORM · EF Core · REST · gRPC

**Architecture** — Microservices · Event-Driven · CQRS · Event Sourcing · Clean / Hexagonal / Onion · DDD · Saga

**Data & Messaging** — PostgreSQL · Redis · Kafka · MySQL · BigQuery

**Cloud & Infra** — Azure · Kubernetes · Docker · AWS · GCP · CI/CD

**Observability** — OpenTelemetry · Datadog · Kibana

---

## Contact

- 🌐 Blog — [williammacarini.com.br](https://www.williammacarini.com.br)
- 💼 LinkedIn — [william-macarini](https://www.linkedin.com/in/william-macarini-288aa5189)
- 📫 Email — [wpmacarini@hotmail.com](mailto:wpmacarini@hotmail.com)

---

<div align="center">

### Core stack

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### Data, cloud & messaging

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

</div>

---

<div align="center">

<sub>Senior Software Engineer · Go & .NET · distributed systems, payments and fiscal platforms at scale</sub>

</div>
