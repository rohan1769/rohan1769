<!-- ════════════════════════ HERO ════════════════════════ -->
![Header](https://capsule-render.vercel.app/api?type=venom&color=0:1a1b26,50:24283b,100:bb9af7&height=280&text=Rohan%20Singh&fontSize=60&fontColor=c0caf5&animation=twinkling&desc=I%20design%20the%20systems%20other%20systems%20depend%20on.&descSize=20&descColor=7dcfff&descAlignY=68)

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=19&duration=3200&pause=1000&color=BB9AF7&center=true&vCenter=true&width=720&height=60&lines=%24+whoami+%E2%86%92+backend+%2B+data+%2B+genai+engineer;%24+scale+%E2%86%92+20%2C000%2B+vehicles+%C2%B7+3+TB%2B+pipelines+%C2%B7+3%2C000%2B+doc+RAG;%24+uptime+%E2%86%92+zero-downtime+releases%2C+privacy+by+default" alt="typing"/>

<br/><br/>

<a href="mailto:rhnsngh1999@gmail.com"><img src="https://img.shields.io/badge/Email-1a1b26?style=for-the-badge&logo=gmail&logoColor=f7768e"/></a>&nbsp;
<a href="https://www.linkedin.com/in/rohansinghin"><img src="https://img.shields.io/badge/LinkedIn-1a1b26?style=for-the-badge&logo=linkedin&logoColor=7dcfff"/></a>&nbsp;
<a href="https://portfolio.rhntech.in"><img src="https://img.shields.io/badge/Portfolio-1a1b26?style=for-the-badge&logo=firefox&logoColor=bb9af7"/></a>&nbsp;
<img src="https://img.shields.io/badge/Kolkata,_IN-1a1b26?style=for-the-badge&logo=googlemaps&logoColor=9ece6a"/>

</div>

<br/>

<!-- ════════════════════════ ABOUT ════════════════════════ -->
<img align="right" width="380" src="https://github-readme-stats.vercel.app/api?username=rohan1769&show_icons=true&theme=tokyonight&hide_border=true&bg_color=00000000&title_color=bb9af7&icon_color=7dcfff&text_color=a9b1d6"/>

### 〔 about 〕

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

<!-- ════════════════════════ ARCHITECTURE ════════════════════════ -->
### 〔 the stack, as I'd whiteboard it 〕

```mermaid
%%{init: {'theme':'base','themeVariables':{
  'primaryColor':'#1a1b26','primaryTextColor':'#c0caf5','primaryBorderColor':'#bb9af7',
  'lineColor':'#7dcfff','secondaryColor':'#24283b','tertiaryColor':'#16161e',
  'clusterBkg':'#1f2335','clusterBorder':'#414868','fontFamily':'Fira Code'}}}%%
flowchart LR
    subgraph L1["⚡ INGEST"]
        direction TB
        a1["Java · Spring Boot"] --- a2["Kafka · RabbitMQ · ActiveMQ"] --- a3["SSE + Redis Pub/Sub"]
    end
    subgraph L2["🔄 PIPELINE · 3 TB+"]
        direction TB
        b1["Airflow · Dagster"] --- b2["Parquet checkpoints"] --- b3["20+ sources → 1 schema"]
    end
    subgraph L3["🤖 INTELLIGENCE"]
        direction TB
        c1["RAG · Docling"] --- c2["Qdrant · pgvector"] --- c3["LLaMA 70B · vLLM · agents"]
    end
    subgraph L0["🔐 TRUST — runs beneath everything"]
        d1["Differential Privacy · PII masking · GDPR/CCPA · OpenTelemetry"]
    end
    L1 ==> L2 ==> L3
    L0 -.-> L1 & L2 & L3
```

---

<!-- ════════════════════════ NUMBERS ════════════════════════ -->
### 〔 numbers that survived production 〕

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

<!-- ════════════════════════ PROJECTS ════════════════════════ -->
### 〔 classified builds — codenames only 〕

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

<!-- ════════════════════════ TIMELINE ════════════════════════ -->
### 〔 trajectory 〕

```mermaid
%%{init: {'theme':'base','themeVariables':{
  'cScale0':'#bb9af7','cScale1':'#7dcfff','cScale2':'#9ece6a','cScale3':'#f7768e',
  'primaryTextColor':'#1a1b26','fontFamily':'Fira Code'}}}%%
timeline
    title backend engineer → platform owner → genai builder
    2021 · 22 : HighRadius — SDE Intern : Java EE + React, enterprise fintech
    2022 · 24 : Entiovi — Software Engineer : Real-time fleet at 99% accuracy : Spring Boot + ActiveMQ + Redis
    2024 : ↑ Senior in 16 months : Xafe.ai privacy engine, TB-scale : Project ATLAS ships
    2025 · 26 : GenAI platform era : Namaiste.ai — on-prem RAG : Idéevin V2.0 — multi-agent AI
```

---

<!-- ════════════════════════ STACK ════════════════════════ -->
### 〔 arsenal 〕

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,python,bash,kafka,rabbitmq,redis,mysql,postgres,docker,kubernetes,gcp,azure,jenkins,nginx,linux,git&perline=9" alt="stack"/>

<br/><br/>

<img src="https://img.shields.io/badge/Airflow-1a1b26?style=flat-square&logo=apacheairflow&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Dagster-1a1b26?style=flat-square&logo=dagster&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/Parquet-1a1b26?style=flat-square&logo=apache&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/MinIO-1a1b26?style=flat-square&logo=minio&logoColor=f7768e"/> <img src="https://img.shields.io/badge/LangChain-1a1b26?style=flat-square&logo=langchain&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/Qdrant-1a1b26?style=flat-square&logo=qdrant&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/pgvector-1a1b26?style=flat-square&logo=postgresql&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Ollama-1a1b26?style=flat-square&logo=ollama&logoColor=c0caf5"/> <img src="https://img.shields.io/badge/vLLM-1a1b26?style=flat-square&logo=lightning&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Docling-1a1b26?style=flat-square&logo=readthedocs&logoColor=9ece6a"/> <img src="https://img.shields.io/badge/MCP-1a1b26?style=flat-square&logo=anthropic&logoColor=bb9af7"/> <img src="https://img.shields.io/badge/N8N-1a1b26?style=flat-square&logo=n8n&logoColor=f7768e"/> <img src="https://img.shields.io/badge/OpenTelemetry-1a1b26?style=flat-square&logo=opentelemetry&logoColor=7dcfff"/> <img src="https://img.shields.io/badge/Grafana-1a1b26?style=flat-square&logo=grafana&logoColor=f7768e"/> <img src="https://img.shields.io/badge/Superset-1a1b26?style=flat-square&logo=apachesuperset&logoColor=9ece6a"/>

</div>

---

<!-- ════════════════════════ NOW ════════════════════════ -->
### 〔 currently 〕

<table>
<tr>
<td>

```text
shipping   ▸ Idéevin V2.0 — enterprise multi-agent AI platform
learning   ▸ agentic orchestration patterns (MCP · N8N · LangChain)
deepening  ▸ privacy gateways for LLM inference
exploring  ▸ document AI at scale with Docling
```

</td>
</tr>
</table>

<br/>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=rohan1769&theme=tokyonight&hide_border=true&background=00000000&ring=bb9af7&fire=f7768e&currStreakLabel=7dcfff" width="55%"/>

<br/><br/>

### open to hard problems in **data infra · LLM platforms · distributed systems**

<a href="mailto:rhnsngh1999@gmail.com"><img src="https://img.shields.io/badge/→_let's_talk-rhnsngh1999@gmail.com-f7768e?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1a1b26"/></a>

</div>

![Footer](https://capsule-render.vercel.app/api?type=venom&color=0:bb9af7,50:24283b,100:1a1b26&height=140&section=footer)
