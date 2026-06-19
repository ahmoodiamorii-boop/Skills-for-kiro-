# 🧠 Kiro Skills Library — 100 Agent Skills for Every Layer of Your Stack

A complete, production-ready collection of **100 agent skills** for [Kiro](https://kiro.dev) — organized, opinionated, and ready to drop into any project.

Each skill turns Kiro into a specialist for that domain: it knows the right patterns, the right standards, and exactly what to deliver.

---

## ⚡ Quick Install

Copy the skills to Kiro's global skills directory and they'll be available in **every project** on your machine:

**Mac/Linux:**
```bash
cp -r .kiro/skills/* ~/.kiro/skills/
```

**Windows (PowerShell):**
```powershell
Copy-Item -Recurse -Force .kiro\skills\* $env:USERPROFILE\.kiro\skills\
```

Or clone directly into your global skills folder:
```bash
git clone https://github.com/ahmoodiamorii-boop/Skills-for-kiro- ~/.kiro/skills-library
cp -r ~/.kiro/skills-library/.kiro/skills/* ~/.kiro/skills/
```

---

## 📦 What's Inside

100 skills across every layer of a modern software project:

### 🗺️ Planning & Architecture (8 skills)
| Skill | What it does |
|-------|-------------|
| `requirements-analyst` | Converts vague ideas into PRDs, user stories, acceptance criteria |
| `system-architect` | Designs system topology, service boundaries, data flow diagrams |
| `api-contract-designer` | Designs OpenAPI/GraphQL schemas before any code is written |
| `database-schema-designer` | ERDs, normalization, indexing strategy, partitioning plans |
| `domain-modeler` | DDD bounded contexts, aggregates, entities, value objects |
| `tech-stack-selector` | Evaluates and recommends languages, frameworks, infra |
| `capacity-planner` | Estimates compute, storage, bandwidth needs at scale |
| `dependency-mapper` | Audits third-party libs, licenses, risk surface |

### 🎨 Frontend (13 skills)
| Skill | What it does |
|-------|-------------|
| `ui-component-builder` | Builds reusable component libraries (React/Vue/Svelte) |
| `page-screen-assembler` | Composes components into full pages and views |
| `state-management` | Zustand/Redux/Pinia stores, derived state, hydration |
| `routing` | Client-side routing, guards, lazy loading, nested routes |
| `form-validation` | Forms with Zod/Yup/react-hook-form schema validation |
| `animation-transition` | Framer Motion, CSS transitions, skeleton loaders |
| `accessibility` | ARIA roles, keyboard nav, WCAG 2.2 compliance |
| `responsive-design` | Breakpoints, mobile-first layouts, fluid typography |
| `internationalization` | i18n setup, locale files, RTL support |
| `theme-design-tokens` | CSS variables, dark/light mode, brand token systems |
| `frontend-performance` | Code splitting, tree shaking, CLS/LCP fixes |
| `pwa` | Service workers, offline caching, push notifications |
| `seo` | Meta tags, OG tags, structured data, sitemaps |

### ⚙️ Backend (17 skills)
| Skill | What it does |
|-------|-------------|
| `rest-api` | CRUD endpoints, versioning, pagination, filtering |
| `graphql` | Schema, resolvers, dataloaders, subscriptions |
| `websocket-realtime` | Socket.io/WS servers, rooms, presence, broadcasting |
| `authentication` | JWT, OAuth2, session management, refresh token rotation |
| `authorization` | RBAC, ABAC, permission matrices, policy enforcement |
| `business-logic` | Domain service layer, use cases, orchestration |
| `event-driven` | Event bus setup, publishers, consumers, event schemas |
| `background-jobs` | BullMQ/Sidekiq queues, cron jobs, dead letter queues |
| `file-upload` | Multipart handling, S3/R2, virus scanning, CDN URLs |
| `email-service` | Transactional templates, Resend/SES integration |
| `sms-push-notifications` | Twilio, FCM/APNs, notification preferences |
| `webhooks` | Inbound/outbound webhooks, HMAC signing, retry |
| `rate-limiting` | Per-user/IP throttling, sliding window, Redis-backed |
| `search` | Elasticsearch/Typesense/Meilisearch, indexing, ranking |
| `caching` | Redis cache layers, invalidation strategies, TTL design |
| `payments` | Stripe/Paddle, subscription billing, webhooks, refunds |
| `audit-log` | Immutable event trail, tamper detection |

### 🗄️ Database & Data (10 skills)
`migration` · `seed-data` · `query-optimizer` · `orm-query-builder` · `replication-failover` · `backup-recovery` · `data-warehouse` · `data-lake` · `cache-warming` · `data-anonymization`

### 🚀 DevOps & Infrastructure (13 skills)
`cicd-pipeline` · `containerization` · `orchestration` · `infrastructure-as-code` · `cloud-provisioning` · `secret-management` · `environment-config` · `dns-cdn` · `load-balancer` · `auto-scaling` · `artifact-registry` · `feature-flags` · `blue-green-canary`

### 🧪 Testing (12 skills)
`unit-test` · `integration-test` · `e2e-test` · `component-test` · `api-test` · `load-stress-test` · `chaos-engineering` · `security-penetration-test` · `accessibility-test` · `visual-regression` · `mutation-test` · `contract-test`

### 📊 Monitoring & Observability (10 skills)
`metrics` · `logging` · `tracing` · `alerting` · `dashboards` · `uptime-monitor` · `error-tracking` · `performance-profiling` · `cost-monitoring` · `anomaly-detection`

### 🔒 Security (9 skills)
`sast` · `dast` · `dependency-vulnerability` · `container-security` · `network-security` · `compliance` · `encryption` · `iam-hardening` · `incident-response`

### 📖 Documentation (8 skills)
`api-docs` · `architecture-docs` · `code-comment` · `changelog` · `onboarding-docs` · `runbook` · `data-dictionary` · `postmortem`

### 🤖 AI/ML (7 skills)
`prompt-engineering` · `rag-pipeline` · `fine-tuning` · `model-evaluation` · `ai-gateway` · `vector-db` · `llm-observability`

### 🔄 Cross-Cutting (10 skills)
`code-review` · `refactoring` · `dependency-upgrade` · `technical-debt` · `scaffolding` · `monorepo` · `opentelemetry` · `multi-tenancy` · `localization-qa` · `data-privacy`

---

## 🛠️ How Skills Work

Each skill lives in its own folder with a `skill.md` file:

```
.kiro/skills/
  authentication/
    skill.md       ← role, responsibilities, output format, standards
  payments/
    skill.md
  ...
```

The `skill.md` defines:
- **Role** — what persona Kiro takes on
- **Responsibilities** — specific tasks the skill handles
- **Output Format** — exactly what deliverables to produce
- **Standards** — hard rules and best practices to enforce

When you invoke a skill in Kiro, the agent loads that context and operates as a specialist for that domain.

---

## 💡 Usage Example

In Kiro chat, reference a skill directly:

```
Using the authentication skill, implement JWT refresh token rotation for my Express app
```

```
Using the database-schema-designer skill, design the schema for a multi-tenant SaaS
```

```
Using the e2e-test skill, write Playwright tests for the checkout flow
```

---

## 🤝 Contributing

Got a skill that's missing? PRs welcome.

1. Fork the repo
2. Create a folder: `.kiro/skills/your-skill-name/`
3. Add a `skill.md` following the existing format
4. Open a PR with a short description of what the skill does

**Skill format:**
```markdown
---
name: Your Skill Name
description: One line description of what this skill does
---

You are a [Role] Agent. Your job is to...

## Responsibilities
- ...

## Output Format
- ...

## Standards
- ...
```

---

## ⭐ If this saved you time, star the repo

More skills, better standards, faster builds — that's the goal.

[![GitHub stars](https://img.shields.io/github/stars/ahmoodiamorii-boop/Skills-for-kiro-?style=social)](https://github.com/ahmoodiamorii-boop/Skills-for-kiro-)
