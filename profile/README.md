# timo-goetz-ai — AI Engineering Platform

> **Automation + KI** · Self-hosted · Hetzner + Vercel · Stand: April 2026

---

## Platform Overview

Vier eigenständige Projekte, aufgeteilt aus einem Monolith (April 2026):

| Projekt | Status | URL | Stack |
|--------|--------|-----|-------|
| [public-site](https://github.com/timo-goetz-ai/public-site) | ✅ Live | [timo-goetz-ai.de](https://timo-goetz-ai.de) | Astro 4 · Vercel |
| [content-studio](https://github.com/timo-goetz-ai/content-studio) | 🚧 Phase 1 | app.timo-goetz-ai.de | Next.js 15 · Supabase · Vercel |
| ops-dashboard | 🚧 Phase 3 | ops.automation-plus-ki.de | Next.js 15 · Coolify |
| infra-dashboard | 🚧 Phase 2 | infra.automation-plus-ki.de | Next.js 15 · Coolify |

---

## Infrastruktur

```
Hetzner VPS (46.224.145.109)
├── Coolify          — Deployment-Platform (15 Apps)
├── n8n              — Automation Workflows
├── Grafana + Loki   — Monitoring + Logging
├── Supabase         — Postgres + Auth + Storage (self-hosted)
├── Authentik        — SSO für interne Services
└── Control Center   — agents.automation-plus-ki.de
```

---

## Was gerade passiert (April 2026)

- **Platform Split:** Dashboard-Monolith (48 Pages, 84 API Routes) → 4 eigenständige Repos
- **Supabase** ersetzt NocoDB/Directus als primärer Data-Layer
- **content-studio** in Entwicklung: SaaS mit Stripe-Billing, Supabase Auth
- **GitHub Org Migration** abgeschlossen: alle Repos jetzt unter `timo-goetz-ai`

---

## Roadmap

```
✅ Phase 0  — Supabase Foundation + Schema Migration
🚧 Phase 1  — content-studio UI + Vercel Deploy + DNS (app.timo-goetz-ai.de)
⏳ Phase 2  — infra-dashboard Monitoring-Pages ausbauen
⏳ Phase 3  — ops-dashboard verschlanken
⏳ Phase 4  — NocoDB/Directus dekommissionieren
```

---

## Abgeschlossen ✅

- Control Center live (`agents.automation-plus-ki.de`) — 07.04.2026
- GitHub Org Migration (5 Repos in timo-goetz-ai) — 07.04.2026
- Alle 15 Apps in Coolify migriert (von mcp-ops docker-compose) — 27.02.2026
- Homestack vollständig deployed auf Hetzner — 02.03.2026
- AI Voice Platform live (`voice.automation-plus-ki.de`) — Phase 1-6 ✅
- AppFlowy live (`appflowy.automation-plus-ki.de`) — 05.03.2026
- Bruno API Tests: 92/92 grün — 03.2026

---

## Repos

| Repo | Beschreibung |
|------|-------------|
| [core-platform](https://github.com/timo-goetz-ai/core-platform) | Admin Dashboard (Next.js 14) + Python APIs |
| [control-center](https://github.com/timo-goetz-ai/control-center) | AI Agent Interface (Next.js 15 + FastAPI) |
| [public-site](https://github.com/timo-goetz-ai/public-site) | Portfolio + Pricing (Astro 4) |
| [content-studio](https://github.com/timo-goetz-ai/content-studio) | Content SaaS (Next.js 15 + Supabase) |
| [smart-note-mcp](https://github.com/timo-goetz-ai/smart-note-mcp) | MCP Server: Smart Notes |
| [mcp-productivity-suite](https://github.com/timo-goetz-ai/mcp-productivity-suite) | MCP Server Suite |

---

<sub>Deployed on Hetzner · CI/CD via GitHub Actions → Coolify · Secrets in 1Password</sub>
