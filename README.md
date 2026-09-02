<div align="center">

# Rahul Nayak

### Backend Engineer in Progress · Systems · GenAI Applications

**Computer Science @ NIT Rourkela**

Building backend systems, developer tools, and infrastructure-heavy projects while exploring how LLMs fit into real production applications.

[![GitHub](https://img.shields.io/badge/GitHub-RahulNayak6467-181717?style=flat-square\&logo=github)](https://github.com/RahulNayak6467)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rahul_Nayak-0A66C2?style=flat-square\&logo=linkedin)](https://www.linkedin.com/in/rahul-nayak-78b414320/)
[![LeetCode](https://img.shields.io/badge/LeetCode-V8M72JYqDX-FFA116?style=flat-square\&logo=leetcode\&logoColor=black)](https://leetcode.com/u/V8M72JYqDX/)

</div>

---

## `whoami`

```ts
const rahul = {
  role: "CS Undergraduate",
  university: "NIT Rourkela",

  interests: [
    "Backend Engineering",
    "Distributed Systems",
    "GenAI Applications",
    "Developer Infrastructure",
  ],

  currentlyLearning: [
    "System Design",
    "Docker & Cloud Infrastructure",
    "Go",
    "Production Backend Engineering",
  ],

  philosophy: "Build it. Break it. Understand why it broke.",
};
```

I started primarily with frontend development, but my focus has shifted heavily toward **backend engineering and systems**.

I enjoy projects where I have to think about things like:

* API and database design
* queues and background workers
* caching and rate limiting
* concurrency
* large file processing
* microservices
* observability
* infrastructure and deployment
* LLM-powered backend systems

---

## `currently-building`

### Transflow

> A large-scale video processing and transcoding platform built to explore production backend architecture.

The goal is not simply to upload and convert videos — I'm using the project to understand how real asynchronous processing systems are designed.

**Planned system**

```text
Client
  │
  ▼
API Gateway / Backend
  │
  ├── Upload Service ───────► Object Storage
  │
  ├── Job Service
  │      │
  │      ▼
  │   Queue / Event Bus
  │      │
  │      ▼
  │   Transcoding Workers
  │
  └── PostgreSQL / Redis

          │
          ▼
   Monitoring + Logs
```

**Exploring through Transflow**

`TypeScript` · `Node.js` · `Express` · `PostgreSQL` · `Redis` · `BullMQ` · `Docker` · `AWS` · `CI/CD` · `Terraform`

Later stages will explore:

`Go` · `Kafka` · `gRPC` · `Kubernetes` · `Observability`

---

## `projects`

<table>
<tr>
<td width="50%" valign="top">

### 🛰️ OrbitX

Satellite tracking platform built during a hackathon with separate **TypeScript and Python backend services**.

The backend periodically retrieves satellite orbital data, stores historical information, and exposes APIs consumed by a 3D satellite visualization frontend.

**Engineering involved**

* TypeScript API
* Python orbital computation service
* PostgreSQL
* scheduled data ingestion
* TLE / SATCAT processing
* multi-service deployment
* Vercel + Render + Railway

</td>

<td width="50%" valign="top">

### 🆘 ResQify

Emergency-management platform for hotels supporting **Guest, Staff and Admin** workflows.

Uses LLM APIs to classify incidents and assist with emergency handling while maintaining role-specific dashboards and alerts.

**Stack**

`React` · `TypeScript` · `Express` · `Supabase` · `Groq` · `Gemini`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### 📈 Quanton

Stock-market dashboard with live market information, gainers and losers, watchlists, and realtime updates.

**Stack**

`React` · `TypeScript` · `TanStack Query` · `Supabase` · `FMP API`

</td>

<td width="50%" valign="top">

### ⚙️ Project Scaffolder

Node.js CLI for generating project structures and automating repetitive project setup.

Built while exploring Node's filesystem APIs and CLI tooling.

**Stack**

`Node.js` · `JavaScript` · `fs` · `npm`

</td>
</tr>
</table>

<div align="center">

[Explore all repositories →](https://github.com/RahulNayak6467?tab=repositories)

</div>

---

## `engineering-stack`

### Backend

<p>
<img src="https://skillicons.dev/icons?i=ts,nodejs,express,postgres,redis&theme=dark" />
</p>

### Frontend

<p>
<img src="https://skillicons.dev/icons?i=react,nextjs,vite,tailwind&theme=dark" />
</p>

### Infrastructure & Tools

<p>
<img src="https://skillicons.dev/icons?i=docker,git,github,linux,aws&theme=dark" />
</p>

### Currently Exploring

<p>
<img src="https://skillicons.dev/icons?i=go,kubernetes,kafka,terraform&theme=dark" />
</p>

---

## `what-im-learning`

My current learning is centered around moving from **"I can build an API"** toward **"I understand how backend systems behave in production."**

```text
Backend
├── API design
├── PostgreSQL
├── caching
├── queues
├── concurrency
├── background processing
└── authentication

Systems
├── Docker
├── distributed systems
├── microservices
├── Kafka
├── Kubernetes
├── gRPC
└── observability

Cloud
├── AWS
├── CI/CD
├── Terraform
└── production deployments

Languages
├── TypeScript  ███████████░
├── JavaScript  ███████████░
└── Go          ███░░░░░░░░
```

---

## `next-up`

Alongside Transflow, I'm learning **Go** with the goal of eventually building an interpreter from scratch.

The idea is to understand more than syntax — particularly:

* parsing
* lexing
* ASTs
* evaluation
* language runtimes
* Go interfaces
* error handling
* idiomatic Go project structure

---

## `github`

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=RahulNayak6467&show_icons=true&hide_border=true&hide_rank=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9" />

<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=RahulNayak6467&hide_border=true&background=0d1117&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff&sideLabels=c9d1d9&currStreakNum=c9d1d9&sideNums=c9d1d9&dates=8b949e" />

</div>

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=RahulNayak6467&bg_color=0d1117&color=c9d1d9&line=58a6ff&point=ffffff&area=true&hide_border=true" />

</div>

---

## `connect`

I'm always interested in talking about backend engineering, interesting systems, developer tooling, and ambitious projects.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/rahul-nayak-78b414320/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge\&logo=github)](https://github.com/RahulNayak6467)
[![LeetCode](https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge\&logo=leetcode\&logoColor=black)](https://leetcode.com/u/V8M72JYqDX/)

<br/>

<sub>Building systems one broken deployment at a time.</sub>

</div>
