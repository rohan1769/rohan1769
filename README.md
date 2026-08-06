<!-- ═══════════════════════════════ HERO ═══════════════════════════════ -->
![Header](https://capsule-render.vercel.app/api?type=waving&color=0:16161e,25:1a1b26,55:414868,80:7aa2f7,100:bb9af7&height=310&text=ROHAN%20SINGH&fontSize=68&fontColor=c0caf5&fontAlignY=32&stroke=bb9af7&strokeWidth=1&desc=Backend%20%E2%9C%A6%20Data%20Platforms%20%E2%9C%A6%20GenAI%20Infrastructure&descSize=22&descColor=7dcfff&descAlignY=52&animation=fadeIn)

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=900&color=BB9AF7&center=true&vCenter=true&width=780&height=64&lines=Spring+Boot+microservices+that+track+20%2C000%2B+vehicles+live;Airflow+pipelines+moving+3+TB%2B+for+World+Bank+%C2%B7+Stanford+research;Self-hosted+LLM+platforms+%E2%80%94+RAG%2C+agents%2C+zero+data+leaves+the+building" alt="typing"/>

<br/>

<!-- ── nav ── -->
<a href="#-how-i-think--the-stack-as-id-whiteboard-it"><img src="https://img.shields.io/badge/🧠_ARCHITECTURE-1a1b26?style=for-the-badge"/></a>
<a href="#-arsenal"><img src="https://img.shields.io/badge/⚙_ARSENAL-1a1b26?style=for-the-badge&logoColor=bb9af7"/></a>
<a href="#-flagship-builds"><img src="https://img.shields.io/badge/🚀_BUILDS-1a1b26?style=for-the-badge"/></a>
<a href="#-trajectory"><img src="https://img.shields.io/badge/🧭_TRAJECTORY-1a1b26?style=for-the-badge"/></a>
<a href="#-numbers-that-survived-production"><img src="https://img.shields.io/badge/📟_IMPACT-1a1b26?style=for-the-badge"/></a>

<br/><br/>

<a href="mailto:rhnsngh1999@gmail.com"><img src="https://img.shields.io/badge/Email-f7768e?style=flat-square&logo=gmail&logoColor=1a1b26"/></a>
<a href="https://www.linkedin.com/in/rohansinghin"><img src="https://img.shields.io/badge/LinkedIn-7dcfff?style=flat-square&logo=linkedin&logoColor=1a1b26"/></a>
<a href="https://portfolio.rhntech.in"><img src="https://img.shields.io/badge/Portfolio-bb9af7?style=flat-square&logo=firefox&logoColor=1a1b26"/></a>
<img src="https://img.shields.io/badge/Kolkata,_India-9ece6a?style=flat-square&logo=googlemaps&logoColor=1a1b26"/>

</div>

<br/>

<!-- ═══════════════════════════════ ABOUT ═══════════════════════════════ -->
<img align="right" width="380" src="https://github-readme-stats.vercel.app/api?username=rohan1769&show_icons=true&theme=tokyonight&hide_border=true&bg_color=00000000&title_color=bb9af7&icon_color=7dcfff&text_color=a9b1d6"/>

## ⌘ About

```yaml
role:      Senior Software Engineer @ Entiovi
years:     4+ in production distributed systems
arc:       Java backend → Data platforms → GenAI infra
promoted:  in 16 months, for end-to-end ownership

trusted_by:
  - World Bank & Stanford research programs
  - US enterprise & fintech clients

principles:
  - runtime-configurable > hardcoded
  - resumable > restartable
  - self-hosted models > leaking data
```

<br clear="right"/>

---

<!-- ═══════════════════════════════ ARCHITECTURE ═══════════════════════════════ -->
## 🧠 How I think — the stack as I'd whiteboard it

> The Arsenal below lists *what* I use. This is *how it fits together* — every system I've shipped follows this shape.

```mermaid
%%{init: {'theme':'base','themeVariables':{
  'primaryColor':'#1f2335','primaryTextColor':'#c0caf5','primaryBorderColor':'#bb9af7',
  'lineColor':'#7dcfff','secondaryColor':'#24283b','tertiaryColor':'#16161e',
  'clusterBkg':'#16161e','clusterBorder':'#414868','fontFamily':'Fira Code'}}}%%
flowchart LR
    subgraph L1["⚡ INGEST"]
        direction TB
        a1["Java · Spring Boot<br/>microservices"] --- a2["Kafka · RabbitMQ<br/>ActiveMQ"] --- a3["SSE + Redis Pub/Sub<br/>stateless streaming"]
    end
    subgraph L2["🔄 PIPELINE · 3 TB+"]
        direction TB
        b1["Airflow · Dagster<br/>orchestration"] --- b2["Parquet checkpoints<br/>resumable by design"] --- b3["20+ sources<br/>→ 1 canonical schema"]
    end
    subgraph L3["🤖 INTELLIGENCE"]
        direction TB
        c1["RAG · Docling<br/>dense + sparse retrieval"] --- c2["Qdrant · pgvector<br/>vector knowledge layer"] --- c3["LLaMA 70B · vLLM<br/>multi-agent, self-hosted"]
    end
    subgraph L0["🔐 TRUST — runs beneath everything"]
        d1["Differential Privacy · PII masking · column encryption · GDPR/CCPA · OpenTelemetry"]
    end
    L1 ==> L2 ==> L3
    L0 -.-> L1 & L2 & L3

    classDef layer fill:#1f2335,stroke:#414868,stroke-width:1.5px,color:#c0caf5
    classDef trust fill:#16161e,stroke:#f7768e,stroke-width:1.5px,color:#f7768e
    class a1,a2,a3,b1,b2,b3,c1,c2,c3 layer
    class d1 trust
```

---

<!-- ═══════════════════════════════ ARSENAL ═══════════════════════════════ -->
## ⚙ Arsenal

> Not a wall of icons — this is where my depth actually sits.

<table>
<tr>
<td width="34%" valign="top" align="center">

### 🏗️ Backend & Microservices
<sub>**PRIMARY WEAPON · 4+ YEARS**</sub>

`████████████████░` 

<img src="https://img.shields.io/badge/Java-1a1b26?style=for-the-badge&logo=openjdk&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Spring_Boot-1a1b26?style=for-the-badge&logo=springboot&logoColor=9ece6a"/>
<img src="https://img.shields.io/badge/Microservices_Architecture-1a1b26?style=for-the-badge&logoColor=bb9af7"/>
<img src="https://img.shields.io/badge/Hibernate_/_JPA-1a1b26?style=flat-square&logo=hibernate&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Spring_MVC-1a1b26?style=flat-square&logo=spring&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/REST_APIs-1a1b26?style=flat-square&logoColor=c0caf5"/> <img src="https://img.shields.io/badge/Concurrency_&_Multithreading-1a1b26?style=flat-square&logoColor=f7768e"/>

<sub>*Event-driven services, LLD/HLD, design patterns — the layer everything else here stands on.*</sub>

</td>
<td width="33%" valign="top" align="center">

### 🤖 AI & GenAI Systems
<sub>**CURRENT FRONTIER · SHIPPING NOW**</sub>

`██████████████░░░`

<img src="https://img.shields.io/badge/RAG_Pipelines-1a1b26?style=for-the-badge&logo=databricks&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/Multi--Agent_Systems-1a1b26?style=for-the-badge&logo=probot&logoColor=7dcfff"/>
<img src="https://img.shields.io/badge/LLM_Serving_·_vLLM_·_Ollama-1a1b26?style=for-the-badge&logo=lightning&logoColor=f7768e"/>
<img src="https://img.shields.io/badge/LangChain-1a1b26?style=flat-square&logo=langchain&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/LLaMA_70B-1a1b26?style=flat-square&logo=meta&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Docling_·_Document_AI-1a1b26?style=flat-square&logo=readthedocs&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/Qdrant-1a1b26?style=flat-square&logo=qdrant&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/pgvector-1a1b26?style=flat-square&logo=postgresql&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/MCP-1a1b26?style=flat-square&logo=anthropic&logoColor=c0caf5"/> <img src="https://img.shields.io/badge/N8N-1a1b26?style=flat-square&logo=n8n&logoColor=f7768e"/>

<sub>*Dense + sparse retrieval, agent orchestration, privacy-gated inference — all self-hosted.*</sub>

</td>
<td width="33%" valign="top" align="center">

### 🔄 Data Engineering
<sub>**TERABYTE-SCALE · OWNED END-TO-END**</sub>

`███████████████░░`

<img src="https://img.shields.io/badge/Apache_Airflow-1a1b26?style=for-the-badge&logo=apacheairflow&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Dagster-1a1b26?style=for-the-badge&logo=dagster&logoColor=bb9af7"/>
<img src="https://img.shields.io/badge/ETL_/_ELT_·_Batch_+_Incremental-1a1b26?style=for-the-badge&logoColor=9ece6a"/>
<img src="https://img.shields.io/badge/Parquet-1a1b26?style=flat-square&logo=apache&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/Python-1a1b26?style=flat-square&logo=python&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/MinIO_S3-1a1b26?style=flat-square&logo=minio&logoColor=f7768e"/> <img src="https://img.shields.io/badge/dlt-1a1b26?style=flat-square&logoColor=c0caf5"/> <img src="https://img.shields.io/badge/Data_Modeling-1a1b26?style=flat-square&logoColor=bb9af7"/>

<sub>*Checkpointed, resumable, runtime-configurable pipelines — 20+ sources, one canonical schema.*</sub>

</td>
</tr>
<tr>
<td valign="top" align="center">

### 📡 Distributed & Messaging
<sub>**BATTLE-TESTED AT FLEET SCALE**</sub>

`███████████████░░`

<img src="https://img.shields.io/badge/Kafka-1a1b26?style=flat-square&logo=apachekafka&logoColor=c0caf5"/> <img src="https://img.shields.io/badge/RabbitMQ-1a1b26?style=flat-square&logo=rabbitmq&logoColor=f7768e"/> <img src="https://img.shields.io/badge/ActiveMQ-1a1b26?style=flat-square&logo=apache&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/Redis_·_Cache_+_Pub/Sub-1a1b26?style=flat-square&logo=redis&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Server--Sent_Events-1a1b26?style=flat-square&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Event--Driven_Architecture-1a1b26?style=flat-square&logoColor=bb9af7"/>

</td>
<td valign="top" align="center">

### ☁️ Cloud & DevOps
<sub>**ZERO-DOWNTIME BY DEFAULT**</sub>

`█████████████░░░░`

<img src="https://img.shields.io/badge/Docker-1a1b26?style=flat-square&logo=docker&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Kubernetes-1a1b26?style=flat-square&logo=kubernetes&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/GCP-1a1b26?style=flat-square&logo=googlecloud&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/Azure-1a1b26?style=flat-square&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Jenkins_CI/CD-1a1b26?style=flat-square&logo=jenkins&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Nginx-1a1b26?style=flat-square&logo=nginx&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/Linux-1a1b26?style=flat-square&logo=linux&logoColor=c0caf5"/>

</td>
<td valign="top" align="center">

### 🔐 Security & Observability
<sub>**PRIVACY IS A FEATURE, NOT A PATCH**</sub>

`██████████████░░░`

<img src="https://img.shields.io/badge/Differential_Privacy-1a1b26?style=flat-square&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Column--Level_Encryption-1a1b26?style=flat-square&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/GDPR_/_CCPA-1a1b26?style=flat-square&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/OpenTelemetry-1a1b26?style=flat-square&logo=opentelemetry&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Grafana-1a1b26?style=flat-square&logo=grafana&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Apache_Superset-1a1b26?style=flat-square&logo=apachesuperset&logoColor=9ece6a"/>

</td>
</tr>
</table>

---

<!-- ═══════════════════════════════ NUMBERS ═══════════════════════════════ -->
## 📟 Numbers that survived production

<div align="center">

<table>
<tr>
<td align="center" width="25%"><h2>🛰️ 2×</h2><b>10K → 20K+ vehicles</b><br/><sub>real-time fleet, re-architected<br/>ingestion + caching paths</sub></td>
<td align="center" width="25%"><h2>🗄️ 3 TB+</h2><b>data ingested</b><br/><sub>legislative, judicial & global<br/>macro data on GCP</sub></td>
<td align="center" width="25%"><h2>🎯 99%</h2><b>data accuracy</b><br/><sub>bulk fleet ops — debugged<br/>live in production</sub></td>
<td align="center" width="25%"><h2>⚡ 30–40%</h2><b>faster syncs</b><br/><sub>parallelized DAGs,<br/>two-phase pipelines</sub></td>
</tr>
<tr>
<td align="center"><h2>🧱 40%+</h2><b>memory reclaimed</b><br/><sub>Parquet checkpoint staging,<br/>fully resumable pipelines</sub></td>
<td align="center"><h2>📚 3,000+</h2><b>docs in RAG</b><br/><sub>LLaMA 70B, fully on-prem,<br/>zero external API calls</sub></td>
<td align="center"><h2>🌍 20+</h2><b>sources unified</b><br/><sub>World Bank · IMF · GDELT<br/>WTO · Meltwater</sub></td>
<td align="center"><h2>🔻 0</h2><b>downtime releases</b><br/><sub>K8s rolling deploys,<br/>health probes, replicas</sub></td>
</tr>
</table>

</div>

---

<!-- ═══════════════════════════════ BUILDS ═══════════════════════════════ -->
## 🚀 Flagship Builds

<table>
<tr>
<td width="50%" valign="top">

#### 🌐 Project ATLAS &nbsp;<sub><sup>`World Bank · Stanford`</sup></sub>
*Global data-intelligence pipeline*

Incremental ETL on Airflow unifying **20+ heterogeneous global sources** — economic, trade, media & conflict data — into one canonical schema for research teams.

`▸` Parallelized DAGs → **30% faster sync**
`▸` DS model runs wired straight into the DAG flow
`▸` End-to-end **OpenTelemetry** observability

<sub>`Airflow` · `Python` · `Azure` · `MinIO` · `OTel`</sub>

</td>
<td width="50%" valign="top">

#### 🔐 Xafe.ai &nbsp;<sub><sup>`Platform Owner`</sup></sub>
*Privacy-preserving ETL engine*

Middleware-controlled ETL where *everything* is runtime-configurable — new sources onboard with **zero code changes**.

`▸` Differential Privacy: dynamic PII masking + column-level encryption
`▸` Parquet checkpoints → **40%+ memory cut**, resumable
`▸` SSE + Redis Pub/Sub → stateless, horizontally scalable

<sub>`Spring Boot` · `Airflow` · `Parquet` · `K8s` · `GDPR/CCPA`</sub>

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🏛️ Project CAPITOL &nbsp;<sub><sup>`US Enterprise`</sup></sub>
*Legislative & judicial data intelligence*

Two-phase Airflow pipeline (raw sync → normalize/enrich) over **3 TB+** of US legislative, Senate & court data — with graceful API-throttle handling, while mentoring a small data team.

`▸` **40% sync-time reduction** on GCP
`▸` Document AI: **Docling + Qdrant** semantic retrieval
`▸` MinIO S3-compatible raw data lake

<sub>`Airflow` · `Docling` · `Qdrant` · `RabbitMQ` · `GCP`</sub>

</td>
<td width="50%" valign="top">

#### 🦙 Namaiste.ai → Idéevin V2.0
*Self-hosted GenAI → enterprise multi-agent AI*

RAG over **3,000+ documents** on **LLaMA 70B** — fully on-premise, not a single external LLM call. Now building the successor.

`▸` Dense + sparse chunking, sequence-tracked IDs
`▸` RabbitMQ-decoupled, fault-tolerant microservices
`▸` V2.0: Dagster + dlt · pgvector · privacy gateway · **vLLM**

<sub>`LLaMA 70B` · `vLLM` · `LangChain` · `pgvector` · `Dagster`</sub>

</td>
</tr>
</table>

---

<!-- ═══════════════════════════════ TRAJECTORY ═══════════════════════════════ -->
## 🧭 Trajectory

> Four stops. Each one a bigger system than the last.

```mermaid
%%{init: {'theme':'base','themeVariables':{
  'primaryColor':'#1f2335','primaryTextColor':'#c0caf5','primaryBorderColor':'#bb9af7',
  'lineColor':'#565f89','fontFamily':'Fira Code','fontSize':'14px',
  'clusterBkg':'#16161e','clusterBorder':'#414868'}}}%%
flowchart LR
    S1(("🎓")) ==> S2(("⚙️")) ==> S3(("📈")) ==> S4(("🤖"))

    S1 --- N1["<b>2021 – 22 · HighRadius</b><br/>SDE Intern<br/><i>Java EE + React,<br/>enterprise fintech delivery</i>"]
    S2 --- N2["<b>2022 – 24 · Entiovi</b><br/>Software Engineer<br/><i>Real-time fleet platform<br/>Spring Boot · ActiveMQ · Redis</i>"]
    S3 --- N3["<b>2024 · Promoted in 16 mo</b><br/>Senior Software Engineer<br/><i>Owned Xafe.ai privacy engine<br/>+ Project ATLAS delivery</i>"]
    S4 --- N4["<b>2025 – now · GenAI Era</b><br/>Platform Builder<br/><i>Namaiste.ai on-prem RAG<br/>→ Idéevin V2.0 multi-agent AI</i>"]

    N2 -.-> A2[/"🎯 99% accuracy · 20K+ vehicles"/]
    N3 -.-> A3[/"🔐 GDPR/CCPA at TB scale · 🌍 20+ sources"/]
    N4 -.-> A4[/"📚 3,000+ doc RAG · 🦙 LLaMA 70B · vLLM"/]

    classDef stop fill:#bb9af7,stroke:#7dcfff,stroke-width:3px,color:#1a1b26,font-weight:bold
    classDef card fill:#1f2335,stroke:#414868,stroke-width:1.5px,color:#c0caf5
    classDef win fill:#16161e,stroke:#9ece6a,stroke-width:1px,color:#9ece6a,font-style:italic

    class S1,S2,S3,S4 stop
    class N1,N2,N3,N4 card
    class A2,A3,A4 win
```

<div align="center">
<sub>

**intern** ─── writes features&nbsp;&nbsp;→&nbsp;&nbsp;**engineer** ─── scales systems&nbsp;&nbsp;→&nbsp;&nbsp;**senior** ─── owns platforms&nbsp;&nbsp;→&nbsp;&nbsp;**builder** ─── ships AI products

</sub>
</div>

---

<!-- ═══════════════════════════════ NOW + STATS ═══════════════════════════════ -->
## 🌱 Currently

```text
shipping   ▸ Idéevin V2.0 — enterprise multi-agent AI platform
learning   ▸ agentic orchestration patterns (MCP · N8N · LangChain)
deepening  ▸ privacy gateways for LLM inference
exploring  ▸ document AI at scale with Docling
```

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=rohan1769&theme=tokyonight&hide_border=true&background=00000000&ring=bb9af7&fire=f7768e&currStreakLabel=7dcfff" width="55%"/>

<br/><br/>

### open to hard problems in **data infra · LLM platforms · distributed systems**

<a href="mailto:rhnsngh1999@gmail.com"><img src="https://img.shields.io/badge/→_let's_talk-rhnsngh1999@gmail.com-f7768e?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1a1b26"/></a>

</div>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:bb9af7,20:7aa2f7,55:414868,100:16161e&height=140&section=footer)
