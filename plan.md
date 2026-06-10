# 1-Year Plan: Get Hired at NAV IT

> **Goal:** Junior developer position at NAV IT (Teknologiavdelingen)
> **Starting point:** JavaScript/TypeScript, C#, teaching experience, 1 merged PR in navikt codebase

---

## Your Strengths Going In

- Merged PR in `navikt/familie-tilbake-frontend` — you've already shipped code to their systems
- TypeScript/JavaScript — their main frontend language
- C# and OOP — transfers directly to Kotlin mentally
- Teaching experience — shows deep understanding, not just surface knowledge; maps directly to psychological safety, team dynamics, and conflict handling
- Based in Oslo — no remote complications

## The Gap

- No production backend experience
- Limited Kotlin/Java
- No hands-on Kubernetes/NAIS
- Limited testing discipline
- No formal exposure to NAV's product development methodology

---

## Months 1–3 — Deepen What You Already Have

### Goals

- [ ] Write strict TypeScript — generics, utility types (`Partial`, `Pick`, `Record`), type narrowing
- [ ] Understand React deeply — not just making things work, but why
- [ ] Learn TanStack Query (NAV uses it in familie-tilbake-frontend)
- [ ] Write tests as a habit — Vitest + React Testing Library
- [ ] Read and understand the familie-tilbake-frontend codebase end to end
- [ ] Read *Gode produkter* by Ida Aalen — understand NAV's product development method

### Specific Skills

**TypeScript**
- Strict mode (`"strict": true` in tsconfig)
- Generic functions and components
- Discriminated unions
- Zod for runtime validation (NAV uses it)

**React**
- `useReducer` and when to use it over `useState`
- Custom hooks — extract and reuse logic
- TanStack Query — fetching, caching, invalidation
- React Hook Form (NAV uses it)

**Testing**
- Unit test pure functions with Vitest
- Component tests with React Testing Library
- Test behaviour, not implementation

**NAV's Product Development Method**
- Read [*Gode produkter*](https://idaaa.no/bestill-bok/) by Ida Aalen (she works at NAV — direct insider source)
- Understand the user-first, iterative MVP cycle: talk to users → sketches/hypotheses → MVP → test → repeat
- Be able to explain *why* you involve users before coding, not just that you do
- Understand the difference between Scrum/Kanban and NAV's product development approach

### ✅ Project: Quick Win — NextJS + GitHub Actions + Vercel

> Specifically recommended by NAV's Principal Officer.

- Create a new NextJS project and publish it to GitHub
- Set up a GitHub Actions workflow that builds the project with NPM on every push
- Deploy to Vercel (free tier)
- Be able to explain clearly: **why is continuous integration important?**

**Why:** Fast to complete (1–2 days), directly fulfills insider advice, and gives you a clean CI/CD example to reference in interviews.

### ✅ Project: Personal Finance Tracker (Frontend)

Build a clean frontend app in React + strict TypeScript that:
- Fetches and displays data from a public API
- Uses TanStack Query for data fetching
- Has form input validated with Zod + React Hook Form
- Has at least 80% test coverage with Vitest
- Uses NAV's Aksel design system components (public npm package)

**Why:** Mirrors the exact stack used in familie-tilbake-frontend. Forces you to use the tools for real.

---

## Months 4–6 — Learn the Backend Side

### Goals

- [ ] Get comfortable with Kotlin syntax and idioms
- [ ] Build a REST API with Kotlin + Spring Boot
- [ ] Connect it to a PostgreSQL database
- [ ] Understand how a BFF (Backend for Frontend) works — you've already read one
- [ ] Learn basic Kubernetes concepts hands-on (`kubectl`, pods, deployments, services)
- [ ] Set up a GitHub Actions CI/CD pipeline

### Specific Skills

**Kotlin**
- Kotlin basics (1–2 weeks — your C# transfers fast)
- Data classes, sealed classes, extension functions
- Coroutines basics
- Spring Boot with Kotlin — controllers, services, repositories

**PostgreSQL**
- Basic SQL (you likely know some already)
- Flyway for database migrations (NAV standard)
- JPA/Hibernate with Kotlin

**Kubernetes / NAIS**
- Read nais.io documentation end to end
- Understand: pods, deployments, services, ingress, configmaps, secrets
- Learn `kubectl get`, `kubectl logs`, `kubectl describe`
- Understand how SIGTERM fits into the pod lifecycle (you already know this conceptually)

**GitHub Actions**
- Write a workflow that runs tests on push
- Build and push a Docker image
- Basic deployment pipeline

### ✅ Project: Full-Stack Workout Tracker (you already have the C# version)

Rebuild your WorkoutTracker as a full-stack project:
- **Backend:** Kotlin + Spring Boot + PostgreSQL
- **Frontend:** React + TypeScript (connect to your own API)
- **Auth:** Simple JWT or session-based
- **CI/CD:** GitHub Actions pipeline that runs tests on push
- **Deploy:** Railway, Render, or Fly.io (free tiers available)

**Why:** You already know the domain. Focus on the new stack, not figuring out what to build. A real deployed app is far more impressive than a tutorial project.

---

## Months 7–9 — Go Deeper Into the NAV Ecosystem

### Goals

- [ ] Make at least 3 more contributions to navikt repos
- [ ] Understand Kafka at a conceptual and basic practical level
- [ ] Read and understand NAV's architecture decisions (ADRs)
- [ ] Get comfortable reading Kotlin codebases you didn't write
- [ ] Start following NAV IT people on LinkedIn — understand their culture

### Specific Skills

**Kafka**
- What it is and why NAV uses it (async messaging between microservices)
- Producers and consumers
- Topics and consumer groups
- You don't need to master it — understand it well enough to talk about it

**Open Source Contributions**
- Browse `github.com/navikt` for repos with good first issues
- Focus on: TypeScript/React repos and Kotlin repos
- Small is fine — docs, tests, bug fixes, small features
- Each PR gets your name known inside the organisation

**Architecture and Systems**
- Read about microservices and why NAV uses them
- Understand how familie-tilbake-frontend talks to familie-tilbake (the Kotlin backend)
- Read about the BFF pattern — you already understand it from server.ts

### ✅ Project: Contribute a Feature to an Open Source navikt Repo

Pick a navikt repo with a clear open issue and implement it properly:
- Write tests for your change
- Handle edge cases
- Write a clear PR description explaining what and why

**Why:** This is the highest-value thing you can do for your application. Every merged PR is a reference they can read before your interview.

---

## Months 10–12 — Apply and Prepare

### Goals

- [ ] Apply for junior developer position at NAV IT
- [ ] Prepare your portfolio — GitHub profile clean and presentable
- [ ] Prepare for technical interview
- [ ] Prepare for team/culture interview — this is equally important at NAV
- [ ] Frame your teaching experience as an asset, not a gap

### Portfolio Checklist

- GitHub profile with pinned repos — the Workout Tracker and Finance Tracker
- Each repo has a proper README with: what it is, why you built it, how to run it
- At least 4–5 merged PRs in navikt repos across the year
- Deployed apps with live links
- The NextJS + Vercel project demonstrating CI/CD understanding

### Technical Interview Preparation

NAV IT does not do whiteboard algorithms. Based on their job listings and culture, they focus on:
- How you think through a problem
- Code quality and testing
- Agile ways of working
- How you collaborate in a team

Prepare to talk about:
- Your merged PRs — what you found, why it mattered, how you fixed it
- Your projects — decisions you made and why
- Testing — how and why you test
- A time you got feedback and changed your approach

### Team & Culture Interview Preparation

NAV actively screens for this. Prepare concrete answers to:

**On teamwork:**
- You contribute socially and technically — not just to your own tasks
- You focus on making the team better, not on being visible
- You create psychological safety (you have direct experience designing this in classrooms)
- You prefer to enable others, but you step up when needed — *never say you want to be team lead*

**On conflict:**
- You resolve conflicts locally first — within the team, not escalated upward immediately
- You listen genuinely before defending your position
- You're not conflict-avoidant — you raise disagreements calmly and constructively
- If the team can't agree, you favour democratic decision-making or bringing in an external expert
- *Never describe yourself as someone who avoids conflict*

**On product development:**
- You understand the user-first principle — design hypotheses and MVPs are tested with real users before building
- You know the difference between building what users ask for and what they actually need
- You can explain why continuous delivery matters (smaller risk, faster feedback)

### Your Unique Angle When Applying

> *"Jeg har undervist programmering i [X] år og har bidratt til navikt-kodebasen — inkludert graceful SIGTERM-håndtering i familie-tilbake-frontend som ble merget av teamet."*

Teaching = you understand fundamentals deeply, and you know how to create environments where people feel safe to fail and learn — which is exactly what psychological safety in a team means.

Open source contributions = you've already passed an informal code review by their own developers.

---

## Quick Reference: NAV IT Tech Stack

| Area | Technology |
|------|-----------|
| Frontend | React, TypeScript, Vite |
| Design system | Aksel (NAV's own) |
| Backend | Kotlin, Java, Spring Boot |
| Messaging | Kafka |
| Database | PostgreSQL |
| Platform | Kubernetes (NAIS) |
| Auth | Azure AD, Wonderwall |
| CI/CD | GitHub Actions |
| Monitoring | Prometheus, Grafana |

---

## Resources

**TypeScript**
- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/)
- [Matt Pocock's Total TypeScript](https://www.totaltypescript.com/)

**React / TanStack**
- [TanStack Query docs](https://tanstack.com/query/latest)
- [React Hook Form docs](https://react-hook-form.com/)

**Kotlin**
- [Kotlin Koans](https://play.kotlinlang.org/koans) — interactive exercises
- [Spring Boot + Kotlin guide](https://spring.io/guides/tutorials/spring-boot-kotlin)

**Kubernetes / NAIS**
- [nais.io](https://nais.io) — NAV's own platform documentation
- [Kubernetes basics](https://kubernetes.io/docs/tutorials/kubernetes-basics/)

**NAV's Product Development Method**
- [*Gode produkter* by Ida Aalen](https://idaaa.no/bestill-bok/) — required reading, written by someone inside NAV
- [detsombetyrnoe.no](https://www.detsombetyrnoe.no) — NAV IT culture and jobs

**NAV IT**
- [github.com/navikt](https://github.com/navikt) — 3000+ open repos to explore and contribute to
