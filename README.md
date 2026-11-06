### Hi, I'm Hartmut 👋

**Founder & builder of Mecurus, DocLayer and RehaTakt · TypeScript, SvelteKit, Next.js, PostgreSQL · multi-agent Claude Code workflows**

I build vertical SaaS products end to end: from the domain model and the written spec, through the UI, to a hardened deployment on my own servers.
Most of the implementation runs through a team of specialised Claude Code agents that I designed for this. The pipeline has hard gates:
CTO review, UX spec, architecture, implementation, QA against the running app, security review and pentest.

#### 🚢 Products

| | What it is | Stack | Code |
|---|---|---|---|
| **DocLayer** | Maritime AI document intelligence for ship managers. AI classification against SFI/ISM taxonomies, vessel and fleet filing, and a bilingual RAG assistant that cites its sources. About 7,300 automated test cases; in pilot. | SvelteKit · PostgreSQL/pgvector · Claude API · Docker | private |
| **RehaTakt** | Administration software for German rehab-sports associations, clubs and instructors. The production system is built by a spec-driven agent factory: 12 module specs, 156 work packages, quality gates with mutation testing, and cross-model review. | TypeScript · Fastify · PostgreSQL 16 (RLS) · React | [prototype](https://github.com/hmomec/rehatakt-prototype) · factory private |
| **Logo Hunt** | Invite-only partnership network: consent-first warm introductions, intro bounties, a credit ledger for closed deals, and an operator console. | Next.js 16 · React 19 · TypeScript · Tailwind v4 | [logohunt](https://github.com/hmomec/logohunt) |
| **Mecurus** | B2B sourcing marketplace with tenders, offers, orders and Stripe payments, built with an agency team. | Laravel · Next.js · MySQL | private |

#### 🤖 How I build

[**claude-code-agent-team**](https://github.com/hmomec/claude-code-agent-team): nine Claude Code sub-agents and the pipeline rules that make them work together.

```text
PRD → CTO review → UX spec + architecture → backend · frontend · DevOps → QA after every task → security review → pentest
```

Three rules I added after real incidents in production:

- No control may claim an effect the server does not deliver, or a restriction the server does not impose.
- HTTP-level tests are not UI verification; someone has to open the screen.
- Every agent reports what it did **not** test.

#### 🧰 Toolbox

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SvelteKit](https://img.shields.io/badge/SvelteKit-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=flat-square&logo=hetzner&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=claude&logoColor=white)

#### 🔭 Currently

- DocLayer pilot: v2.14 adds OCR for scanned PDFs (including German) and Excel text extraction
- RehaTakt release 1, built work package by work package through the factory
