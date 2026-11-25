<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Raviraj%20Sonar&fontSize=56&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20%C2%B7%20Distributed%20Systems%20%C2%B7%20AI%20Engineering&descAlignY=60&descSize=18" width="100%" alt="Raviraj Sonar" />

**Final-year B.Tech student at MIT Academy of Engineering, Pune, building scalable backends, real-time systems and AI-powered platforms.**

[![Resume](https://img.shields.io/badge/Resume-Download%20PDF-2ea44f?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](https://github.com/RavirajSonar40/RavirajSonar40/raw/main/Raviraj_Sonar_Resume.pdf)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raviraj-sonar-4b5574370/)
[![Email](https://img.shields.io/badge/Email-Get%20in%20touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sonarraviraj60@gmail.com)

</div>

---

## About

I build backend-heavy products end to end: schema design, APIs, real-time delivery, caching, queues, and, more recently, LLM pipelines with retrieval and agentic workflows. My work ranges from a system for the **PCMC Traffic Police that was recognised by the Chief Minister of Maharashtra**, to a **zero-downtime PostgreSQL migration engine benchmarked at 10M+ rows**.

| | |
|---|---|
| **Education** | B.Tech, Electronics & Telecommunication Engineering, MIT Academy of Engineering, Pune (2023 – 2027), CGPA 8.45 / 10 |
| **Focus areas** | Backend architecture, database design, distributed systems, RAG and agentic AI |
| **Currently** | Building **Report Buddy** and agentic AI / RAG systems |
| **Recognition** | Winner, Coday Hackathon (NICE Technologies) · 300+ DSA problems on LeetCode |
| **Open to** | Internships and entry-level roles in backend, full-stack and AI engineering |

---

## Tech Stack

**Languages**

<img src="https://skillicons.dev/icons?i=java,js,ts,py&perf" alt="Languages" />

**Frontend and frameworks**

<img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,tailwind,angular,fastapi&perf" alt="Frameworks" />

**Databases**

<img src="https://skillicons.dev/icons?i=postgres,mongodb,mysql,redis,prisma&perf" alt="Databases" />

`pgvector` · `Pinecone` · `Mongoose`

**Messaging and real-time**

<img src="https://skillicons.dev/icons?i=kafka,rabbitmq,graphql&perf" alt="Messaging" />

`BullMQ` · `Socket.IO` · `gRPC` · `REST` · `SSE` · `WebSockets`

**DevOps and cloud**

<img src="https://skillicons.dev/icons?i=linux,docker,kubernetes,nginx,aws,cloudflare,git,github&perf" alt="DevOps" />

**AI / ML**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-8A2BE2?style=flat-square)
![Vector Search](https://img.shields.io/badge/Vector%20Search-0077B6?style=flat-square)
![Ragas](https://img.shields.io/badge/Ragas%20Evaluation-FF6F00?style=flat-square)
![Multi-provider LLMs](https://img.shields.io/badge/Multi--provider%20LLMs-111111?style=flat-square)
![XGBoost](https://img.shields.io/badge/XGBoost-2E8B57?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas%20%7C%20NumPy-150458?style=flat-square&logo=pandas&logoColor=white)

**Core CS:** DSA · OOP · Operating Systems · Computer Networks · DBMS · System Design · Distributed Systems
**Security and tools:** JWT · RBAC · Postman · Figma · Cursor · Antigravity · OpenCode · Hermes

---

## Featured Projects

### 🚦 Traffic Buddy: WhatsApp-first traffic complaint platform
*Built for PCMC Traffic Police · Mar 2025 – May 2025*

> 🏆 **Recognised by the Chief Minister of Maharashtra** for improving the complaint handling workflow of the PCMC Traffic Police through automated routing, real-time status tracking and streamlined resolution.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-FF4438?style=flat-square)
![Cloudflare R2](https://img.shields.io/badge/Cloudflare%20R2-F38020?style=flat-square&logo=cloudflare&logoColor=white)

- Citizens file complaints over **WhatsApp (Twilio)**; officers and administrators work from a dashboard backed by **REST APIs** and **JWT-based RBAC**.
- **Geolocation-based routing** assigns each complaint automatically.
- Evidence is compressed with **Sharp** and stored in **Cloudflare R2**; dashboards are faster thanks to **MongoDB indexing** and **Redis cache-aside** caching.
- **Redis distributed locking** guarantees single ownership of a complaint, **Socket.IO** pushes real-time updates, and **BullMQ** sends WhatsApp notifications asynchronously.

```mermaid
flowchart LR
    A[Citizen on WhatsApp] --> B[Twilio]
    B --> C[Node.js API<br/>JWT + RBAC]
    C --> D[Geolocation routing]
    C <--> E[(MongoDB)]
    C <--> F[(Redis<br/>cache + locks)]
    C --> G[Sharp] --> H[(Cloudflare R2)]
    C --> I[BullMQ] --> B
    C --> J[Socket.IO] --> K[Officer / Admin dashboard]
```

[**Backend →**](https://github.com/RavirajSonar40/TrafficBuddy-Backend) · [**Dashboard →**](https://github.com/RavirajSonar40/TrafficDashbord)

---

### 🔍 Crime Track: crime records and analytics platform
*Jul 2025 – Sep 2025*

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![React](https://img.shields.io/badge/React.js-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Analytics](https://img.shields.io/badge/Analytics-Heatmaps-orange?style=flat-square)

- Designed **normalized PostgreSQL schemas** managing **5,000+ crime records** with high data integrity.
- Optimized complex SQL queries (joins, aggregations), **reducing report generation time by 40%**.
- Built **real-time analytics dashboards and heatmaps** for faster decision-making across **3+ police zones**.

[**Repository →**](https://github.com/RavirajSonar40/crime-track1)

---

### 📝 Report Buddy: FIR management with workflow automation
*Oct 2025 – Present*

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![React](https://img.shields.io/badge/React.js-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![RBAC](https://img.shields.io/badge/Role--Based%20Auth-C0392B?style=flat-square)

- Engineered relational schemas supporting **multi-role access for 100+ users** with strict referential integrity.
- Implemented secure **role-based authentication and authorization**, improving system security by **60%**.
- Developed **end-to-end FIR workflow automation**, **reducing manual processing time by 45%**.

<!-- Add your Report Buddy repo link here: [**Repository →**](https://github.com/RavirajSonar40/<repo-name>) -->

---

## More Projects

<table>
<tr>
<td width="50%" valign="top">

### 🧠 AI Knowledge & Action Platform
**RAG and agentic AI** · *2026*

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)

- Semantic search, **RAG-based Q&A**, document recommendations and **multi-provider LLM** support.
- **LangGraph** workflows with task decomposition, tool execution, evidence gathering, iterative verification and **human-in-the-loop approval**.
- **Ragas-based evaluation and observability**: faithfulness, context precision, recall, latency and token usage in an **Angular dashboard**.

<!-- Add repo link: [Repository →](https://github.com/RavirajSonar40/<repo-name>) -->

</td>
<td width="50%" valign="top">

### 🔄 SafeMigrate
**Zero-downtime PostgreSQL migration engine** · *2025*

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)

- **Logical replication / WAL (pgoutput)** with asynchronous shadow-table backfilling for live workloads.
- **Kafka-ordered change replay** and **Redis checkpoints** for idempotent crash recovery and atomic cutover with zero data loss.
- Benchmarked at **10M+ rows**: **11,655 rows/sec**, 14.30 min backfill, **zero failures**, validated with fault injection and checksum verification.

<!-- Add repo link: [Repository →](https://github.com/RavirajSonar40/<repo-name>) -->

</td>
</tr>
</table>

---

## Experience

| Role | Company | Period |
|------|---------|--------|
| **Machine Learning Engineer Intern** | Univ.Ai (Remote) | Jun 2025 – Jul 2025 |
| **WordPress Developer Intern** | Canspirits.Ai (Remote) | Jun 2024 – Jul 2024 |

- **Univ.Ai:** Built and evaluated Decision Tree and XGBoost models for loan default prediction, with preprocessing, feature engineering and EDA in Pandas and NumPy.
- **Canspirits.Ai:** Customized and maintained client WordPress sites, deployed on Bluehost with routine backups and maintenance.

---

## Achievements

- 🥇 **Winner, Coday Hackathon (NICE Technologies):** greedy and dynamic programming solution
- 🏛️ **Recognised by the Chief Minister of Maharashtra** for Traffic Buddy
- 🧩 **300+ DSA problems** solved on LeetCode (arrays, trees, graphs, DP)
- ⚡ **10M+ row zero-failure migration benchmark** with SafeMigrate

---

## GitHub Stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=RavirajSonar40&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=RavirajSonar40&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />

</div>

---

<div align="center">

### Let's connect

Open to internships, collaborations and interesting engineering problems.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raviraj-sonar-4b5574370/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sonarraviraj60@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-2ea44f?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](https://github.com/RavirajSonar40/RavirajSonar40/raw/main/Raviraj_Sonar_Resume.pdf)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%" alt="" />

</div>