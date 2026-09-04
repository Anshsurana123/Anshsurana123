<div align="center">

# ⚡ ANSH SURANA

### `AI Systems` · `Infrastructure` · `Security` · `Edge AI`

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=22&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=750&lines=I+build+systems%2C+not+just+demos.;I+like+breaking+my+own+software.;AI+%C3%97+Infrastructure+%C3%97+Security+%C3%97+Automation;Build.+Measure.+Break.+Fix.+Ship." />

<br>

[![GitHub](https://img.shields.io/badge/GitHub-Anshsurana123-181717?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/Anshsurana123)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://linkedin.com/in/yourprofile)
[![Email](https://img.shields.io/badge/Email-anshsuran01%40gmail.com-EA4335?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:anshsuran01@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-000000?style=for-the-badge\&logo=vercel\&logoColor=white)](https://portfolio-website-rho-five-80.vercel.app/)

<img src="https://komarev.com/ghpvc/?username=Anshsurana123&style=for-the-badge&color=58A6FF&label=PROFILE+VIEWS" />

</div>

---

<div align="center">

> **I don't just use abstractions.**
>
> **Sometimes I build what's underneath them.**

</div>

---

## 🧠 `$ whoami`

```text
┌─────────────────────────────────────────────────────────┐
│                                                         │
│  ANSH SURANA                                            │
│                                                         │
│  ▸ AI systems                                           │
│  ▸ Retrieval & ranking                                  │
│  ▸ Backend infrastructure                               │
│  ▸ Security engineering                                 │
│  ▸ Edge / Android AI                                    │
│  ▸ Developer tooling                                    │
│                                                         │
│  Current loop:                                          │
│                                                         │
│       BUILD → MEASURE → BREAK → FIX → SHIP             │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

I like working on the layer where things stop being magic and start becoming engineering.

Vector indexes.
Retrieval pipelines.
Authentication protocols.
Agent execution.
Android internals.
Real-time systems.

Basically:

**if something interesting is happening underneath the API, I probably want to know how it works.**

---

# 🚀 Things I've Built

<div align="center">

### 🧠 SYSTEMS

**`vector-db-from-scratch`**

### ⚡ AI

**`RAGINGOA`**

### 🔐 SECURITY

**`Bitfrost`**

### 📱 EDGE

**`Jagrut`**

### 🔎 INTELLIGENCE

**`Sentinel`**

### 🎯 RANKING

**`Job Recruitment`**

</div>

---

# 🧠 `vector-db-from-scratch`

### A vector database built from scratch in Rust.

**HNSW · WAL · Snapshots · Recovery · PQ · Filtering · Concurrency**

This is probably the project that best represents how I like to build.

Instead of wrapping an existing vector database, I implemented the machinery underneath it.

```text
                    ┌───────────────┐
                    │    Client     │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │   API Layer   │
                    └───────┬───────┘
                            │
                 ┌──────────┴──────────┐
                 ▼                     ▼
          ┌──────────────┐      ┌──────────────┐
          │ HNSW Search  │      │   Filtering  │
          └──────┬───────┘      └──────┬───────┘
                 │                     │
                 └──────────┬──────────┘
                            ▼
                    ┌───────────────┐
                    │ Vector Store  │
                    └───────┬───────┘
                            │
                  ┌─────────┴─────────┐
                  ▼                   ▼
             ┌────────┐          ┌──────────┐
             │  WAL   │          │ Snapshot │
             └────┬───┘          └─────┬────┘
                  └─────────┬──────────┘
                            ▼
                       Crash Recovery
```

### What makes it interesting

* HNSW approximate nearest-neighbor search
* optimized distance calculations
* metadata filtering
* tombstones and compaction
* product quantization
* WAL persistence
* snapshot recovery
* concurrent read/write workloads
* actual recall and latency gates
* crash-recovery testing

`Rust` `HNSW` `WAL` `PQ` `Concurrency`

---

# ⚡ `RAGINGOA`

### Retrieval engineering, not “just another RAG app.”

**FAISS HNSW · Embeddings · Reranking · Guardrails · Multilingual · STT**

The pipeline is designed around measurable retrieval latency and layered safety rather than a single `retrieve → prompt → answer` call.

```text
Input
  │
  ▼
Language / STT
  │
  ▼
Guardrails
  │
  ▼
Embedding
  │
  ▼
FAISS HNSW
  │
  ▼
Hybrid Retrieval
  │
  ▼
Reranking
  │
  ▼
Evidence
  │
  ▼
Generation
  │
  ▼
Post-check
  │
  ▼
Response
```

The repository includes reproducible retrieval benchmark artifacts with measured latency breakdowns and percentile statistics.

`Python` `FAISS` `HNSW` `Embeddings` `Reranking`

---

# 🔐 `Bitfrost`

### An AI/API gateway built around identity, request protection and reliability.

**HMAC · Replay Protection · Rate Limiting · Circuit Breaker · Cache · Telemetry**

The interesting part isn't forwarding an API request.

It's everything that can go wrong around one.

```text
Client
  │
  ▼
Identity
  │
  ├── HMAC
  ├── Timestamp
  ├── Replay Protection
  └── Tenant Validation
           │
           ▼
      Policy Layer
           │
      ┌────┴────┐
      ▼         ▼
    Cache    Upstream
      │         │
      └────┬────┘
           ▼
       Telemetry
```

`Go` `HMAC-SHA256` `Supabase` `WebSockets` `Gateway`

---

# 📱 `Jagrut`

### An Android assistant that actually touches the operating system.

**Wake Word · ONNX/TFLite · Hinglish · Accessibility · Camera2 · Automation**

Instead of stopping at conversational AI, Jagrut connects language understanding to real Android capabilities.

```text
Voice
  │
  ▼
Wake Word
  │
  ▼
STT
  │
  ▼
Command Parser
  │
  ├───────────────┐
  ▼               ▼
Local Action    AI Planner
  │               │
  └───────┬───────┘
          ▼
    Action Validation
          │
          ▼
 Android Execution
```

Built around Android internals such as `AccessibilityService`, Camera2, and on-device model runtimes.

`Kotlin` `Android` `ONNX Runtime` `AccessibilityService` `Camera2`

---

# 🔎 `Sentinel`

### Academic intelligence + claim lineage.

Sentinel combines academic document processing with a structured claim relationship model.

The interesting bit isn't simply generating an answer.

It's being able to reason about:

**Where did this claim come from?**
**What supports it?**
**What depends on it?**
**What is connected to it?**

```text
Source
  │
  ▼
Document
  │
  ▼
Claim
  │
 ┌┴─────────────┐
 ▼              ▼
Parent        Children
 │              │
 └──────┬───────┘
        ▼
   Evidence Graph
```

`Next.js` `React` `Prisma` `Supabase` `Gemini`

---

# 🎯 `Job Recruitment`

### Hybrid retrieval + deterministic ranking + reranking.

Rather than asking an LLM to simply “score this candidate,” the system separates retrieval and ranking into distinct stages.

```text
Candidate
   │
   ├───────────────┐
   ▼               ▼
Lexical         Semantic
Retrieval       Retrieval
   │               │
   └───────┬───────┘
           ▼
      Hybrid Score
           │
           ▼
   Deterministic Rules
           │
           ▼
    Cross-Encoder
           │
           ▼
      Final Ranking
```

`Python` `BM25` `Embeddings` `Cross-Encoder` `Docker`

---

# 🧪 The Rest of the Lab

Not every experiment deserves a giant section.

But they're here:

| Project                                                                              | What it explores                                                     |
| ------------------------------------------------------------------------------------ | -------------------------------------------------------------------- |
| [Collaborative Workspace](https://github.com/Anshsurana123/collaborative-workspace)  | Real-time collaboration, synchronization, whiteboards & shared state |
| [DevLens](https://github.com/Anshsurana123/dev-lens-IBM-BOB)                         | AI-assisted repository analysis and developer tooling                |
| [ChronoGuard](https://github.com/Anshsurana123/ChronoGuard)                          | Computer vision, tracking, privacy filtering & real-time events      |
| [Sark Pharma Tech Services](https://github.com/Anshsurana123/sarkpharmatechservices) | Deployed full-stack product                                          |

---

# 🧰 Stack

<div align="center">

### Languages

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge\&logo=rust\&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge\&logo=go\&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge\&logo=typescript\&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge\&logo=kotlin\&logoColor=white)

### AI / Systems

![FAISS](https://img.shields.io/badge/FAISS-005571?style=for-the-badge)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=for-the-badge\&logo=onnx\&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge\&logo=postgresql\&logoColor=white)

### Web / Infrastructure

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge\&logo=nextdotjs\&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge\&logo=supabase\&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge\&logo=docker\&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge\&logo=githubactions\&logoColor=white)

</div>

---

# ⚙️ Current Operating System

```text
┌────────────────────────────────────────────────────────┐
│                                                        │
│  BUILD                                                │
│      ↓                                                 │
│  MEASURE                                               │
│      ↓                                                 │
│  FIND THE UGLY EDGE CASE                               │
│      ↓                                                 │
│  BREAK IT                                               │
│      ↓                                                 │
│  FIX IT                                                 │
│      ↓                                                 │
│  SHIP                                                   │
│      ↺                                                 │
│                                                        │
└────────────────────────────────────────────────────────┘
```

I genuinely enjoy the part where the happy-path demo stops working.

That's usually where the interesting engineering starts.

---

# 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Anshsurana123&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" />

<br>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Anshsurana123&layout=compact&theme=tokyonight&hide_border=true" />

</div>

---

<div align="center">

<img src="https://raw.githubusercontent.com/Anshsurana123/Anshsurana123/output/github-contribution-grid-snake.svg" />

</div>

---

<div align="center">

### `some people collect tabs. I collect unfinished systems.`

<br>

**Build something weird.**

</div>
