### Hi, I'm Pablo 👋

Founder and lead engineer at **[RAVO Company](https://github.com/ravo-company)**, a Brazilian software house building AI-assisted operations software for law firms and real-estate businesses. I take products from the first conversation with the customer to production, and I keep running them after launch.

- 🏗️ I build multi-tenant SaaS on **Next.js / TypeScript / PostgreSQL**: tenant isolation in the database (RLS), forward-only migrations, CI gates and on-call runbooks.
- 🤖 I build AI products where a human stays in control: LLMs propose, people approve, and every write is audited.
- 📈 I spent 5+ years in B2B growth (paid acquisition, CRM, sales operations) before engineering, so I build with the business metric in mind.
- 🎓 Software Engineering @ FIAP (2024–2026) · 📍 Caldas Novas, Brazil (UTC−3) · 🗣️ Portuguese (native), English

---

#### Selected work

Production systems with paying customers. The repositories live in the [ravo-company](https://github.com/ravo-company) organization and are private because of client confidentiality; I can give access for technical interviews.

| Project | What it is | Stack |
|---|---|---|
| **RAVO Suite** | Multi-tenant operations platform for fractional-ownership resorts: sales floor, quota inventory, WhatsApp customer care on the Meta Cloud API, billing and double-entry P&L. 1,450+ tests, 37 hash-frozen migrations, RLS per tenant, staging/production on a VPS with tested restores. | Next.js 15 · React 19 · TypeScript · PostgreSQL 17 · Docker |
| **Legal Ops Portal** | AI-assisted intake and triage of court notices for law firms. Pulls from the national court gazette (DJEN), CNJ DataJud and IMAP mailboxes; Claude drafts the analysis, a controller approves, and only then is the task created in the firm's practice-management system, exactly once. White-label, one silo per firm. | Next.js 14 · Supabase (RLS) · Anthropic API · Vercel + VPS worker |
| **RAVO OS** | Internal operations cockpit: CRM pipeline, MRR/churn, cohorts and LTV, accrual P&L, goals. The database is the API (PostgREST), with auth done in SQL (bcrypt + signed JWT, lockout, rate limiting). | React 18 · TypeScript · Vite · PostgREST · PostgreSQL 16 |

#### How I work

- Small PRs, green CI, written decisions ([ADRs](https://adr.github.io/)) and honest "known debt" sections.
- Security is checked by CI on every change: secret scanning, a gate that fails if an API route has no auth policy, and a scan of client bundles for leaked secrets.
- I work with AI coding agents (Claude Code, Cursor) in isolated worktrees, following a written protocol. Scope, architecture, review and merges are my decisions.

---

📫 **sistema@ravocompany.com.br**
