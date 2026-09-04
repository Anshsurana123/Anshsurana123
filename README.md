<div align="center">

# Ansh Surana

### I build AI systems, infrastructure, and developer tools.

**From vector databases and retrieval systems to Android automation and security infrastructure — I like building the layers underneath the product.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://linkedin.com/in/yourprofile)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:anshsuran01@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge\&logo=vercel\&logoColor=white)](https://portfolio-website-rho-five-80.vercel.app/)

![Profile Views](https://komarev.com/ghpvc/?username=Anshsurana123\&style=flat-square\&label=PROFILE+VIEWS)

</div>

---

## 👋 About Me

I'm a developer who enjoys building the parts that usually get hidden behind abstractions.

My projects tend to sit at the intersection of:

* **AI / ML systems**
* **retrieval & ranking**
* **backend infrastructure**
* **security**
* **Android / edge AI**
* **developer tooling**
* **distributed and real-time systems**

I care about more than getting a demo to work. I like measuring systems, understanding failure modes, and figuring out what happens underneath the API call.

```python
ansh = {
    "location": "India 🇮🇳",
    "languages": ["Rust", "Python", "Go", "TypeScript", "Kotlin"],
    "interests": [
        "AI systems",
        "retrieval & ranking",
        "infrastructure",
        "security",
        "edge AI",
        "developer tools"
    ],
    "current_mode": "build → measure → break → improve"
}
```

---

## 🧰 Tech I Work With

### Languages

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge\&logo=rust\&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge\&logo=go\&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge\&logo=typescript\&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge\&logo=kotlin\&logoColor=white)

### AI / ML / Data

![FAISS](https://img.shields.io/badge/FAISS-005571?style=for-the-badge)
![ONNX Runtime](https://img.shields.io/badge/ONNX_Runtime-005CED?style=for-the-badge\&logo=onnx\&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge\&logo=postgresql\&logoColor=white)

### Web / Mobile

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge\&logo=nextdotjs\&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge\&logo=android\&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge\&logo=tailwindcss\&logoColor=white)

### Infrastructure

![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge\&logo=supabase\&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge\&logo=prisma\&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge\&logo=docker\&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge\&logo=githubactions\&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge\&logo=git\&logoColor=white)

---

# 🔥 Featured Projects

## 🧠 [Vector DB from Scratch](https://github.com/Anshsurana123/vector-db-from-scratch)

**A persistent vector database built in Rust.**

Built from the ground up to explore how modern vector infrastructure actually works.

* **HNSW** approximate nearest-neighbor indexing
* **Optimized distance functions** with manual loop unrolling
* **Metadata filtering** with correctness-preserving fallback behavior
* **WAL + snapshots + crash recovery**
* **Product Quantization** for compressed vector storage
* **Concurrent reads and writes**
* **Benchmark and correctness gates** for recall, latency, persistence, and recovery

The project includes actual crash-recovery tests and concurrent workloads rather than relying purely on synthetic examples.

`Rust` `HNSW` `WAL` `Product Quantization` `Concurrency`

---

## ⚡ [RAGINGOA](https://github.com/Anshsurana123/RAGINGOA)

**A multilingual retrieval system designed around measurable latency and layered safety.**

* FAISS **HNSW** retrieval
* Embedding + retrieval + reranking pipeline
* Multilingual query processing
* STT integration
* Layered input/output guardrails
* Extractive evidence handling before generative synthesis
* Retrieval benchmarks with recorded **P50 / P95 / P99** measurements

The repository includes the benchmark artifacts used to evaluate the retrieval pipeline and break latency down across its major stages.

`Python` `FAISS` `HNSW` `Embeddings` `Reranking` `Guardrails`

---

## 🔐 [Bitfrost](https://github.com/Anshsurana123/Bitfrost)

**An AI/API gateway focused on identity, request protection, caching, and operational controls.**

* HMAC-based request authentication
* Timestamp / replay protection
* Tenant-aware request handling
* Circuit breaker
* Rate limiting
* Semantic-response caching
* Real-time WebSocket telemetry
* Upstream AI request proxying

Built as an exploration of the security and reliability problems surrounding AI gateways rather than just another API wrapper.

`Go` `HMAC-SHA256` `Supabase` `WebSockets` `API Gateway`

---

## 📱 [Jagrut](https://github.com/Anshsurana123/jagrut)

**An Android assistant built around on-device intelligence and system-level automation.**

* Offline wake-word inference
* ONNX/TFLite model integration
* Hinglish command parsing
* Android `AccessibilityService` automation
* Camera2 integration
* Deterministic local command handling
* AI-assisted action planning
* Explicit action restrictions before execution

The interesting part isn't the chatbot — it's the bridge between natural-language commands and actual Android capabilities.

`Kotlin` `Android SDK` `ONNX Runtime` `AccessibilityService` `Camera2`

---

## 🔎 [Sentinel](https://github.com/Anshsurana123/sentinel)

**An academic intelligence platform combining document analysis with claim and source lineage.**

* Supabase authentication
* Prisma-backed data model
* Academic document processing
* Gemini-powered analysis
* Claim relationships and lineage
* Recursive parent/child claim traversal
* Interactive visualization of evidence relationships
* Modular API routes for separate system concerns

The claim-chain system is designed to preserve relationships between claims rather than treating generated answers as isolated text.

`Next.js` `React` `Prisma` `Supabase` `Gemini`

---

## 🎯 [Job Recruitment](https://github.com/Anshsurana123/job-recruitment)

**A hybrid information-retrieval and ranking pipeline for candidate matching.**

* Lexical + semantic retrieval
* Candidate scoring
* Seniority and experience analysis
* Cross-encoder reranking
* Duplicate / keyword-stuffed content detection
* Deterministic ranking logic
* Validation and evaluation tooling

Rather than asking an LLM to simply "score a resume", the system separates retrieval, scoring, and reranking into distinct stages.

`Python` `Embeddings` `BM25` `Cross-Encoder` `Docker`

---

# 🧪 Other Things I've Built

A few other projects worth exploring:

**[Collaborative Workspace](https://github.com/Anshsurana123/collaborative-workspace)**
Real-time collaborative workspace using synchronization, WebSockets, whiteboards, Kanban, and document-style collaboration.

**[DevLens](https://github.com/Anshsurana123/dev-lens-IBM-BOB)**
AI-assisted repository analysis, code review, security review, documentation, and developer workflows.

**[ChronoGuard](https://github.com/Anshsurana123/ChronoGuard)**
Computer-vision prototype exploring tracking, privacy filtering, geofencing, and real-time events.

**[Sark Pharma Tech Services](https://github.com/Anshsurana123/sarkpharmatechservices)**
A deployed full-stack web platform built with Next.js, TypeScript, and PostgreSQL.

---

# 📈 How I Like to Build

```text
Idea
 ↓
Prototype
 ↓
Measure
 ↓
Find the ugly edge cases
 ↓
Break it
 ↓
Fix it
 ↓
Ship
```

I'm particularly interested in projects where the interesting question isn't just:

> **"Can we make it work?"**

but:

> **"What happens when it fails, scales, gets attacked, or gets pushed past its happy path?"**

---

# 📬 Let's Talk

I'm interested in collaborating on:

**AI systems · retrieval · infrastructure · security · developer tools · Android/edge AI**

📩 **[anshsuran01@gmail.com](mailto:anshsuran01@gmail.com)**

🌐 **[Portfolio](https://portfolio-website-rho-five-80.vercel.app/)**

---

<div align="center">

### Build things worth inspecting.

</div>
