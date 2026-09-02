<!-- ===================== HEADER ===================== -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=130&section=header" width="100%" alt="" />

<div align="center">

# Rahul Nayak

<a href="YOUR_LINKEDIN_URL">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&duration=2800&pause=900&color=6C63FF&center=true&vCenter=true&width=520&height=40&lines=Backend+Developer;CS+%40+NIT+Rourkela;Building+Transflow+in+TypeScript;Learning+Go+and+distributed+systems" alt="Backend Developer · CS @ NIT Rourkela · Building Transflow · Learning Go and distributed systems" />
</a>

Building APIs, queues and infrastructure — and learning how systems behave past the happy path.

<p>
  <img src="https://img.shields.io/badge/Focus-Backend%20Engineering-6C63FF?style=for-the-badge" alt="Focus: Backend Engineering" />
  <img src="https://img.shields.io/badge/Learning-Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Learning Go" />
  <img src="https://img.shields.io/badge/Into-Distributed%20Systems-8A2BE2?style=for-the-badge" alt="Into Distributed Systems" />
</p>

<p>
  <a href="YOUR_LINKEDIN_URL"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="YOUR_LEETCODE_URL"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
  <a href="mailto:YOUR_EMAIL"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://komarev.com/ghpvc/?username=RahulNayak6467&label=Views&style=flat-square&color=6C63FF" alt="Profile views" />
</p>

</div>

---

## About

I work on the parts of software users never see — APIs, databases, background jobs, caching and deployment. Right now I'm moving past CRUD and figuring out how real backends handle **scale, concurrency and failure**.

```ts
const rahul = {
  role: "Backend Developer",
  education: "CS @ NIT Rourkela",
  workingOn: "Transflow — distributed video transcoding",
  learning: ["Go", "System Design", "AWS", "Kafka"],
  philosophy: "Build → Break → Understand → Improve",
};
```

---

## Tech Stack

**Daily driver**

<p>
  <img src="https://skillicons.dev/icons?i=ts,js,nodejs,express,postgres,redis,docker,git,github,linux&theme=dark" alt="TypeScript, JavaScript, Node.js, Express, PostgreSQL, Redis, Docker, Git, GitHub, Linux" />
  <br>
  <img src="https://img.shields.io/badge/Zed-084CCF?style=flat-square&logo=zedindustries&logoColor=white" alt="Zed" />
  <img src="https://img.shields.io/badge/Bruno-F4AA41?style=flat-square&logo=bruno&logoColor=black" alt="Bruno" />
  <img src="https://img.shields.io/badge/BullMQ-DC382D?style=flat-square" alt="BullMQ" />
  <img src="https://img.shields.io/badge/pnpm-F69220?style=flat-square&logo=pnpm&logoColor=white" alt="pnpm" />
</p>

**Currently learning**

<p>
  <img src="https://skillicons.dev/icons?i=go,aws,kafka&theme=dark" alt="Go, AWS, Kafka" />
</p>

| Area | What I'm after |
| --- | --- |
| **Go** | Idiomatic Go, goroutines, channels, context |
| **System Design** | Caching, queues, service boundaries, failure modes |
| **AWS** | Deploying and operating backend services |
| **Kafka** | Event-driven architecture and log-based messaging |

---

## Projects

### Transflow — Distributed Video Processing Platform

Handles large video uploads and turns them into streamable renditions without blocking the request path.

```text
Client ──▶ API (Express) ──▶ PostgreSQL  (metadata, job state)
              │
              ▼
        Redis + BullMQ ──▶ Transcode Workers ──▶ HLS renditions
                                  │                    │
                          retries · progress           ▼
                                               Object Storage
```

- Chunked uploads for large files, with resumable state in Postgres
- Queue-backed transcoding so the API stays responsive under load
- Worker retries, dead-letter handling and per-job progress tracking
- Multiple quality presets output as HLS for adaptive streaming
- Containerised services with structured logging

<p>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>

🚧 **In progress** · [Repo →](YOUR_TRANSFLOW_REPO)

<br>

### OrbitX — Satellite Tracking & Orbital Data Platform

Ingests real orbital data from **CelesTrak** and computes live satellite positions across two backend services.

```text
CelesTrak (TLE) ──▶ Ingest Job ──▶ PostgreSQL ──▶ Node API ──▶ Next.js
                                                     │  ▲
                                                     ▼  │
                                           Python service (SGP4)
                                     position · velocity · altitude · period
```

- Scheduled TLE ingestion with historical snapshots retained in Postgres
- SGP4 propagation in a separate Python service, called by the Node API
- Derived orbital metrics: altitude, velocity, orbital period, ground track
- Two independently deployed backends behind a single frontend

<p>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white" />
</p>

🏆 **Team hackathon project** · [Repo →](YOUR_ORBITX_REPO)

---

## Currently

```text
├── Building Transflow — upload pipeline and worker reliability
├── Learning Go, starting with concurrency primitives
├── Working through system design fundamentals
└── Daily DSA practice
```

---

## GitHub Activity

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=RahulNayak6467&theme=github_dark" width="96%" alt="GitHub profile summary: contributions, public repos, join date" />

<br><br>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=RahulNayak6467&theme=github_dark" width="47%" alt="Repositories per language" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=RahulNayak6467&theme=github_dark" width="47%" alt="Most committed languages" />

<br><br>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=RahulNayak6467&theme=github_dark" width="47%" alt="Commit, PR and issue stats" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=RahulNayak6467&theme=github_dark&utcOffset=5.5" width="47%" alt="Most productive time of day" />

<br><br>

<img src="https://streak-stats.demolab.com?user=RahulNayak6467&theme=github-dark-blue&hide_border=true" width="70%" alt="Contribution streak: total contributions, current streak, longest streak" />

</div>

<sub>Language and commit charts reflect repository activity, not proficiency.</sub>

---

<div align="center">

## Let's talk

Backend engineering, distributed systems, infrastructure or developer tooling — happy to chat.

<a href="YOUR_LINKEDIN_URL"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="YOUR_LEETCODE_URL"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
<a href="mailto:YOUR_EMAIL"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

<br><br>

`Build → Break → Understand → Improve`

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=130&section=footer" width="100%" alt="" />
