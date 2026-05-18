<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=800&color=58A6FF&center=true&vCenter=true&width=720&lines=Hi%2C+I'm+Mosleh+%F0%9F%91%8B;Full-Stack+Engineer+%26+System+Architect;I+ship+enterprise+systems%2C+not+prototypes.;25%2B+production+repos+%E2%80%A2+Multi-tenant+%E2%80%A2+Fintech+%E2%80%A2+AI" alt="Typing intro" />

<br/>

[![GitHub followers](https://img.shields.io/github/followers/Mosleh92?label=Follow&style=for-the-badge&logo=github&color=58A6FF)](https://github.com/Mosleh92)
[![Profile views](https://komarev.com/ghpvc/?username=Mosleh92&style=for-the-badge&color=58A6FF&label=Profile+Views)](https://github.com/Mosleh92)
[![Email](https://img.shields.io/badge/Email-moslehmohammad2%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:moslehmohammad2@gmail.com)

</div>

---

## 🧑‍💻 About Me

I'm a **full-stack engineer and system architect** who builds **enterprise-grade software that actually ships to production**. My portfolio includes a **15-service microservices architecture** powering a major shopping mall, **multi-tenant SaaS platforms** for the SMB market, and **fintech infrastructure** for currency exchange operators.

I work end-to-end: data model → API → frontend → DevOps → live deployment.

> **Currently open to:** white-label licensing • freelance engagements • technical partnerships

---

## 🏗️ Featured Architecture — Enterprise Mall Operations Platform

A **15-microservice ecosystem** I designed and built for a major UAE shopping mall. Spans operations, CX, tenants, reporting, notifications, wayfinding, and complaints — all production-deployed under a Docker Compose + Traefik infrastructure.

> 📐 **[Read the full architecture blueprint →](https://github.com/Mosleh92/enterprise-mall-architecture)**

```mermaid
graph TB
    subgraph "User Tiers"
        OPS[Operations Staff]
        CX[CX / Management]
        TENANT[Tenants]
        VISITOR[Mall Visitors]
    end

    subgraph "Frontends - React + Vite + PWA"
        OP[Ops Portal]
        CXP[CX Portal]
        TP[Tenant Portal]
        MAP[Digital Wayfinding Map]
        CF[Complaints Form]
    end

    subgraph "Backend APIs - Node.js"
        CORE[Core API<br/>shared business logic]
        OPSA[Ops API<br/>operations-specific]
        WF[Workflow Engine<br/>tasks + roles + RBAC]
        REPORT[Report System<br/>PDF + templates]
        MC[Mall Connect<br/>integrations]
    end

    subgraph "Background Workers"
        NOTIF[Notification Service]
        WA[WhatsApp Integration]
    end

    subgraph "Infrastructure"
        TRAEFIK[Traefik Reverse Proxy]
        DOCKER[Docker Compose]
        TAIL[Tailwind Support]
    end

    OPS --> OP --> OPSA
    CX --> CXP --> CORE
    TENANT --> TP --> CORE
    VISITOR --> MAP
    VISITOR --> CF --> CORE

    OPSA --> CORE
    CORE --> WF
    CORE --> REPORT
    CORE --> MC
    MC --> WA
    WF --> NOTIF

    TRAEFIK -.routes.-> OP & CXP & TP & MAP & CF
    DOCKER -.hosts.-> CORE & OPSA & NOTIF & REPORT
```

**Tech:** Node.js · TypeScript · React · Vite · PWA · Tailwind · Redis · Docker · Traefik · WhatsApp API

---

## 🚀 Public Projects

<table>
<tr>
<td width="50%" valign="top">

### 🏬 [Enterprise Mall Architecture](https://github.com/Mosleh92/enterprise-mall-architecture)
**Blueprint of a 15-service production system**

Real architecture documentation • Mermaid diagrams • Service decomposition

`Architecture` `Microservices` `Enterprise` `Case-Study`

📐 Case study of real client work

</td>
<td width="50%" valign="top">

### 🏦 [Exchange Platform](https://github.com/Mosleh92/exchange-platform)
**Multi-tenant currency exchange & P2P trading**

Real-time WebSocket trading • Role-based access • KYC + escrow

`Node.js` `React` `PostgreSQL` `Supabase` `WebSocket`

⭐ Has community star

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏬 [MallOS Enterprise](https://github.com/Mosleh92/mallos-enterprise)
**AI + IoT mall management system**

2FA multi-role auth • Real-time monitoring • Predictive analytics

`TypeScript` `Node.js` `AI` `IoT`

</td>
<td width="50%" valign="top">

### 🎮 [MallQuest](https://github.com/Mosleh92/MallQuest)
**Hamster-Kombat-style gamification for malls**

4 dashboards • Bilingual (AR/EN) • Real-time reward engine

`Python` `Gamification` `Bilingual` `Real-time`

</td>
</tr>
</table>

---

## 💼 Private Client Work

A summary of production systems delivered under client agreements. Code is private; happy to walk through architecture on request.

| System | Type | Stack |
|---|---|---|
| 🏬 **Mall Operations Platform** | 15-service architecture | Node.js, TypeScript, React, Docker, Traefik |
| 🎫 **Vouchers System** | Full-stack (backend + frontend + mobile) | JavaScript / Node.js |
| 🏘️ **Leasing Management System** | SaaS for real-estate operators | JavaScript / Node.js |
| 🚀 **BizKuasa** | Multi-tenant SaaS (Indonesia) | Node.js, PostgreSQL, Redis |
| 🤖 **WhatsApp Automation** | AI-powered customer engagement | Baileys, Groq, Ollama |

---

## 🛠️ Tech Stack

<div align="center">

#### Languages
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

#### Frameworks & Frontend
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=pwa&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socket.io&logoColor=white)

#### Data & Infrastructure
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefikproxy&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

#### AI & Integrations
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-FF6B35?style=for-the-badge)
![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)
![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Mosleh92&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Mosleh92&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com?user=Mosleh92&theme=tokyonight&hide_border=true" />

</div>

---

## 💼 What I Build For Clients

- **Multi-tenant SaaS backends** — auth, billing, admin tooling, RBAC
- **Microservices architectures** — service boundaries, message queues, infra topology
- **Payment integrations** — PayPal, Xendit, Stripe, crypto, P2P escrow
- **Real-time platforms** — WebSocket + Redis-backed dashboards
- **AI integration layers** — Groq, Ollama, OpenAI, LLaVA
- **Enterprise portals** — React + Vite + PWA frontends, role-aware UX
- **End-to-end Docker deployments** — production-grade on any VPS

---

## ⚖️ A Note on Code Use

All code in this account is **proprietary and copyrighted**. Each repository ships with a `LICENSE` and `NOTICE` declaring terms. Reading, studying, and pattern reference are welcome; commercial use, redistribution, and derivative works require explicit licensing.

If you want to use any of this in your business, **let's talk** — terms are reasonable for legitimate use cases.

---

## 📬 Get In Touch

<div align="center">

[![Email](https://img.shields.io/badge/Email-moslehmohammad2%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:moslehmohammad2@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Mosleh92-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Mosleh92)

**Open to:** Freelance engagements · White-label licensing · Technical partnerships

</div>

---

<div align="center">

⭐ *If any of these projects look interesting, give one a star — it really helps!*

</div>
