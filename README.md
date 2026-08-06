<div align="center">

<a href="https://github.com/Techtalk2806">
<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=3000&pause=1000&color=7C6AFF&center=true&vCenter=true&width=800&height=100&lines=Raju+Mishra;Full-Stack+Engineer+%2B+AI%2FML+Engineer;Building+Production+Healthcare+AI+Systems" alt="Typing SVG" /></a>

<br/>

### Full-Stack Engineer · AI/ML Engineer · Technical Lead

**Distributed systems · AI-driven decisioning · Production infrastructure at scale**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/raju-mishra-599885310)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:educationpoint701@gmail.com)

</div>

---

## About

Technical Lead and sole engineer on a **production healthcare-commerce platform** serving live customer traffic — I own the full stack end to end: backend services, frontend, AI-driven decisioning systems, database architecture, and production infrastructure. No team, no handoffs, no dedicated DevOps.

I build systems the way they're supposed to be built: **audit before implementing, verify root cause before fixing, dry-run every data migration, fail loud on missing config.**

- 🏥 Leading engineering + AI/ML on a confidential production healthcare platform *(details under NDA)*
- 🤖 Shipped AI-driven recommendation engines and automated clinical-verification workflows into live production
- ⚙️ Own end-to-end production infra — multi-process clusters, CI/CD, replica sets, caching layers
- 💬 Ask me about **distributed caching, RBAC design, state machines, MongoDB at scale, OpenAI/LangChain**
- 🎯 Care about correctness over velocity — I find and fix the bugs nobody else noticed were there

---

## Engineering Highlights

Selected production work. Specific client/product names withheld under NDA.

**🧠 AI & Machine Learning**
- Designed an **AI-driven recommendation & substitution engine** — multi-stage aggregation pipeline with hard-constraint filtering, availability-awareness, server-side savings computation, and price-ascending ranking
- Built an **automated clinical-verification workflow** as a strict state machine, hard-gating downstream fulfilment on human expert sign-off — closing a real patient-safety gap
- Diagnosed a silent data-integrity bug where a required-flag was never being read correctly, causing **100% of gated orders to bypass verification undetected**; shipped a derivation engine + dry-run-first backfill to repair historical production data
- Production LLM systems: OpenAI GPT-4 (ChatCompletions, embeddings, function calling, streaming), LangChain, RAG pipelines, persona-driven chatbots with memory

**🔐 Security & Access Control**
- Architected a full **RBAC system from scratch**: isolated admin identity model, 10 roles, resource-level granular permissions, and a complete audit trail on every privileged action
- **Mandatory TOTP 2FA**, short-lived JWTs with permission versioning, rotating refresh tokens, Redis-backed session invalidation
- Security audit that identified and closed **53 previously unguarded admin routes**, plus a router-stack regression test to prevent recurrence
- Field-level PII encryption with a shared, audited decryption pattern applied across every read path

**⚡ Performance & Scale**
- Two-tier caching architecture (in-process LRU + Redis) with **single-flight stampede protection, stale-while-revalidate refresh, and popularity-weighted TTLs** — sustaining a **97% cache-hit rate** in production
- Migrated MongoDB standalone → **replica set** with zero customer-facing downtime; full VPS infrastructure migration across providers, also zero-downtime
- BullMQ background job queues with a dedicated reconciliation worker; write-path optimization taking a hot endpoint from **240ms → 12ms**
- 12-instance clustered API deployment with zero-downtime CI/CD auto-deploy and automatic rollback on failed health checks
- Root-caused a production incident where **5,177 critical slow-query alerts fired in 6 hours** — traced to an unbounded text-search candidate set, fixed via index redesign

**💳 Payments, Compliance & Correctness**
- Took a payment gateway live end-to-end with multi-method support (online, COD, manual international settlement) and dual-currency geo-detected pricing
- Found and fixed a **critical financial bug where tax was being double-counted at checkout** — against statutory tax law — plus a tax-grouping compliance defect that was silently overwriting HSN codes
- Built HMAC-signed, tamper-proof public document links with expiry, and integer-paise-based money arithmetic to eliminate floating-point drift across the platform
- Replaced fragile string-matched geographic serviceability with a precise **20,000+ entry pincode-level lookup**

**🔎 Search & SEO Engineering**
- Owns technical SEO end to end: schema.org structured data, crawlability audits, and elimination of **soft-404s returning HTTP 200** — validated directly in Google Search Console
- Rebuilt platform-wide pagination to be **fully crawlable for the first time**, with per-page canonicals and scroll-position restoration
- Standing architectural lesson from a production incident: **never derive canonical or redirect URLs from `request.url` in Next.js standalone mode**

---

## Tech Stack

**Languages & Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Backend & Data**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-E10098?style=for-the-badge&logo=redis&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

**Infrastructure & DevOps**

![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?style=for-the-badge&logo=pm2&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**AI & Machine Learning**

![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![RAG](https://img.shields.io/badge/RAG_Pipelines-6E56CF?style=for-the-badge)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-FF6B6B?style=for-the-badge)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-F7931E?style=for-the-badge&logo=python&logoColor=white)

---

## Engineering Principles

> These aren't aspirations — they're how I actually work.

- **Audit before implementing.** Verify what's actually shipped, with file-level evidence — never trust a feature's status from memory or a changelog.
- **Root-cause before fixing.** A symptom patched is a bug deferred. Reproduce with `curl`, `mongosh`, and logs before touching code.
- **Dry-run every data migration.** Scripts default to read-only; `--apply` is always an explicit, deliberate flag.
- **Fail loud on config.** Missing environment variables throw at boot, not silently at 3 AM in production.
- **One concern per branch.** Reviewable diffs beat heroic commits.
- **The API is the source of truth for UI state.** Zero client-side business logic duplicating server rules.

---

## Selected Public Work

| Project | Description | Stack |
|---|---|---|
| 💼 [**Job Portal Platform**](https://jobs.wishgeekstechserve.com) | Full job listing & application platform with admin panel | MERN |
| 🛠️ [**Services Dashboard**](https://admin.wishgeeks.com/) | Real-time service workflows, payments & invoicing | MERN |
| 🛒 [**E-commerce Platform**](https://www.wishgeeks.com/) | Cart, checkout & full API integration | MERN |
| ⚖️ [**vKeel**](https://www.vkeel.com/) | Legal consultation booking platform | MERN |
| 🤖 [**Greps.ai**](https://greps.ai/) | SaaS with auth, chatbot integration & API services | MERN |
| 💬 **TulipBot** | AI-powered lead generation & management backend | Node.js, OpenAI |
| 🏨 **Hotel Management System** | Room bookings, seasonal pricing, billing & staff assignment | Node.js, MongoDB |

*Current production work is under NDA and not publicly linkable. Happy to walk through architecture and design decisions in detail on a call.*

---

## GitHub Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=Techtalk2806&show_icons=true&theme=tokyonight&hide_border=true&count_private=true"/>
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Techtalk2806&layout=compact&theme=tokyonight&hide_border=true"/>

</div>

---

<div align="center">

*"Correctness first. Everything else is negotiable."*

![Profile Views](https://komarev.com/ghpvc/?username=Techtalk2806&color=7C6AFF&style=for-the-badge)

</div>
