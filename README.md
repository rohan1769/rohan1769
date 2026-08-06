<!-- ─────────────────────────  HEADER  ───────────────────────── -->
![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0a0e14,45:10151f,100:1f6feb&height=250&section=header&text=Rohan%20Singh&fontSize=52&fontColor=ffffff&fontAlignY=32&desc=Distributed%20Systems%20%C2%B7%20Terabyte-Scale%20Data%20Platforms%20%C2%B7%20GenAI%20Infrastructure&descSize=17&descColor=8b949e&descAlignY=52&animation=fadeIn)

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&multiline=true&repeat=true&width=760&height=75&lines=I+build+backends+that+track+20%2C000%2B+vehicles+in+real+time+%F0%9F%9B%B0%EF%B8%8F;I+move+3+TB%2B+through+pipelines+for+World+Bank+%C2%B7+Stanford+%F0%9F%8C%8D;I+ship+self-hosted+LLM+platforms+%E2%80%94+no+API+keys+leave+the+building+%F0%9F%94%90)](https://git.io/typing-svg)

<br/>

[![Email](https://img.shields.io/badge/rhnsngh1999@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rhnsngh1999@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rohansinghin)
[![Portfolio](https://img.shields.io/badge/portfolio.rhntech.in-0d1117?style=for-the-badge&logo=firefox&logoColor=58a6ff)](https://portfolio.rhntech.in)
[![Location](https://img.shields.io/badge/Kolkata,_India-2ea043?style=for-the-badge&logo=googlemaps&logoColor=white)](#)

</div>

<br/>

<!-- ─────────────────────────  SYSTEM DESIGN OF ME  ───────────────────────── -->
## 🧠 `system-design --of rohan`

> Every engineer has a stack. Here's mine — as the architecture diagram I'd actually draw.

```mermaid
flowchart LR
    subgraph INGEST["⚡ Ingestion Layer — 4+ yrs"]
        A1[Java · Spring Boot]
        A2[Kafka · RabbitMQ · ActiveMQ]
        A3[REST · SSE + Redis Pub/Sub]
    end

    subgraph PIPELINE["🔄 Data Platform — 3 TB+"]
        B1[Apache Airflow · Dagster]
        B2[Parquet Checkpointing]
        B3[Canonical Schema · 20+ sources]
    end

    subgraph AI["🤖 GenAI Layer"]
        C1[RAG · Docling · Qdrant · pgvector]
        C2[LLaMA 70B · vLLM · Ollama]
        C3[Multi-Agent · LangChain · MCP]
    end

    subgraph TRUST["🔐 Trust Layer"]
        D1[Differential Privacy Engine]
        D2[PII Masking · Column Encryption]
        D3[GDPR / CCPA · OpenTelemetry]
    end

    INGEST --> PIPELINE --> AI
    TRUST -.enforced across.- INGEST
    TRUST -.enforced across.- PIPELINE
    TRUST -.enforced across.- AI
```

---

<!-- ─────────────────────────  IMPACT DASHBOARD  ───────────────────────── -->
## 📟 Production Telemetry

<div align="center">

| Metric | Reading | System |
|:---|:---:|:---|
| 🛰️ Fleet scaled | `10K → 20K+ vehicles` | Real-time tracking microservices |
| 🎯 Data accuracy | `99%` | Bulk fleet operations, production |
| 🗄️ Data ingested | `3 TB+` | US legislative / Senate / court data (GCP) |
| 🌍 Sources unified | `20+` | World Bank · IMF · GDELT · WTO · Meltwater |
| ⚡ Sync time cut | `30–40%` | Parallelized Airflow DAGs |
| 🧱 Peak memory saved | `40%+` | Parquet checkpoint staging |
| 📚 Docs in RAG | `3,000+` | Self-hosted, LLaMA 70B, zero external calls |
| 🔻 Downtime on release | `0` | K8s rolling deploys + health probes |

</div>

---

<!-- ─────────────────────────  CAREER TIMELINE  ───────────────────────── -->
## 🧭 Trajectory

```mermaid
timeline
    title Backend Engineer → Data Platform Owner → GenAI Builder
    2021-22 : HighRadius — SDE Intern
            : Java EE + React for enterprise fintech
    2022-24 : Entiovi — Software Engineer
            : Real-time fleet platform · 99% accuracy
            : Spring Boot + ActiveMQ + Redis middleware
    2024 : Promoted to Senior (16 months)
         : Xafe.ai privacy engine · GDPR/CCPA at TB scale
         : GRIPP for World Bank / Stanford
    2025-26 : GenAI Platform Engineering
            : Namaiste.ai — on-prem RAG, LLaMA 70B
            : Idéevin V2.0 — multi-agent enterprise AI
```

---

<!-- ─────────────────────────  FLAGSHIP BUILDS  ───────────────────────── -->
## 🚀 Flagship Builds

<table>
<tr>
<td width="50%" valign="top">

### 🌍 GRIPP
**Global Resilience Intelligence Platform** · *World Bank / Stanford*

Incremental ETL on Airflow unifying **20+ heterogeneous global sources** into one canonical schema for data scientists.

- Parallelized DAGs → **30% faster sync**
- DS model runs wired directly into DAG flow
- End-to-end **OpenTelemetry** observability

`Airflow` `Python` `Azure` `MinIO` `OTel`

</td>
<td width="50%" valign="top">

### 🔐 Xafe.ai
**Privacy-Preserving ETL Engine** · *Platform Owner*

Middleware-controlled ETL where *everything* is runtime-configurable — new sources onboard with **zero code changes**.

- Differential Privacy: dynamic PII masking + column-level encryption
- Parquet checkpoints → **40%+ memory cut**, fully resumable
- SSE + Redis Pub/Sub → stateless, horizontally scalable

`Spring Boot` `Airflow` `Parquet` `K8s` `GDPR/CCPA`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏛️ Semantic Intelligence Platform
**3 TB+ US legislative, Senate & court data** · *GCP*

Two-phase Airflow pipeline (raw sync → normalization/enrichment) with graceful API-throttle handling — while mentoring a small data engineering team.

- **40% sync time reduction**
- Document AI: **Docling + Qdrant** semantic retrieval
- MinIO S3-compatible raw data lake

`Airflow` `Docling` `Qdrant` `RabbitMQ` `GCP`

</td>
<td width="50%" valign="top">

### 🦙 Namaiste.ai → Idéevin V2.0
**Self-hosted GenAI, evolving into multi-agent AI**

RAG over **3,000+ documents** on **LLaMA 70B** — fully on-premise, not a single external LLM call. Now building the enterprise successor.

- Dense + sparse chunking with sequence-tracked IDs
- RabbitMQ-decoupled fault-tolerant microservices
- V2.0: Dagster + dlt ingestion · pgvector · privacy gateway · **vLLM** serving

`LLaMA 70B` `vLLM` `LangChain` `pgvector` `Dagster`

</td>
</tr>
</table>

---

<!-- ─────────────────────────  TECH ARSENAL  ───────────────────────── -->
## 🛠️ Arsenal

<div align="center">

**⚙️ Core Backend**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)

**📡 Distributed & Messaging**

![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![ActiveMQ](https://img.shields.io/badge/ActiveMQ-D22128?style=for-the-badge&logo=apache&logoColor=white)

**🔄 Data Engineering**

![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![Dagster](https://img.shields.io/badge/Dagster-654FF0?style=for-the-badge&logo=dagster&logoColor=white)
![Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=for-the-badge&logo=apache&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72C48?style=for-the-badge&logo=minio&logoColor=white)

**🤖 AI / GenAI**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-24327B?style=for-the-badge&logo=qdrant&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-4B8BBE?style=for-the-badge&logo=lightning&logoColor=white)

**☁️ Cloud & DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

</div>

---

<!-- ─────────────────────────  CURRENTLY  ───────────────────────── -->
## 🌱 Currently Shipping & Learning

```text
🤖 Idéevin V2.0 — multi-agent AI    ██████████████░░  in production build
🔬 Agentic workflows (MCP · N8N)    ████████████░░░░  orchestration patterns
🔐 Privacy gateways for LLMs        ██████████████░░  policy-enforced inference
📄 Document AI (Docling)            █████████████░░░  structured extraction at scale
```

---

<!-- ─────────────────────────  GITHUB STATS  ───────────────────────── -->
## 📊 Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=rohan1769&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=1f6feb&text_color=8b949e&ring_color=58a6ff" width="49%"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rohan1769&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e" width="40%"/>

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=rohan1769&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=30363d&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff)](https://github.com/rohan1769)

</div>

---

<!-- ─────────────────────────  FOOTER  ───────────────────────── -->
<div align="center">

### 💬 Let's Build Something Hard

Open to collaborating on **data engineering**, **ML/LLM infrastructure**, and gnarly **distributed systems** problems.

**Ask me about:** Airflow at scale · Spring Boot microservices · Vector search · Self-hosted LLMs · Differential privacy

<br/>

[![Email](https://img.shields.io/badge/Let's_Talk-rhnsngh1999@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rhnsngh1999@gmail.com)

</div>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:0a0e14,45:10151f,100:1f6feb&height=130&section=footer)
