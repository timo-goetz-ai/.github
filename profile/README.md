# timo-goetz-ai — AI Engineering Platform

> **Automation + KI** · Self-hosted (Hetzner/Coolify) · Produkte auf Vercel wo sinnvoll

[![Portfolio](https://img.shields.io/badge/portfolio-timo--goetz--ai.de-0969da?style=for-the-badge)](https://timo-goetz-ai.de)
[![Control Center CI](https://github.com/timo-goetz-ai/control-center/actions/workflows/build-and-push.yml/badge.svg)](https://github.com/timo-goetz-ai/control-center/actions)

---

## Aktive Repos (Ist 2026-06)

| Projekt | Repo | Status | URL |
| --- | --- | --- | --- |
| Portfolio | [`portfolio`](https://github.com/timo-goetz-ai/portfolio) | Live | [timo-goetz-ai.de](https://timo-goetz-ai.de) |
| Content Studio | [`content-studio`](https://github.com/timo-goetz-ai/content-studio) | Phase 1 | [app.timo-goetz-ai.de](https://app.timo-goetz-ai.de) |
| Control Center | [`control-center`](https://github.com/timo-goetz-ai/control-center) | Live | [agents.automation-plus-ki.de](https://agents.automation-plus-ki.de) |
| Infra / VPS | [`infra-vps`](https://github.com/timo-goetz-ai/infra-vps) | Stacks | Tunnel → `/opt/stacks` |
| Workspace (intern) | [`ai-workspace`](https://github.com/timo-goetz-ai/ai-workspace) | Dev | — |
| Smart Note MCP | [`smart-note-mcp`](https://github.com/timo-goetz-ai/smart-note-mcp) | Tooling | Obsidian MCP + CLI |

## Architektur (3 Säulen)

```
TimoGoetz1988/ai-data     → Governance & Wissen (Volume AI_DATA)
timo-goetz-ai/ai-workspace → Produkt-Code
timo-goetz-ai/infra-vps    → Betrieb (n8n, Qdrant, Hermes, SigNoz)
```

Abgelöst / archiviert: `apki-*`, `ai-agent-platform`, `analytic-dashboard`, `infra-code`, `public-site` / `core-platform` (Namen nur noch in alter Doku).

## Governance auf der Platte

Regeln, Salvage aus Legacy-Repos, Session-Hub: privates Meta-Repo **[TimoGoetz1988/ai-data](https://github.com/TimoGoetz1988/ai-data)** (nicht unter der Org).

---

<sub>Hetzner · Coolify · GitHub Actions · Secrets in 1Password · Org-Mapping: `REGISTRY/timo-goetz-ai-org-abgleich.md` im ai-data-Repo</sub>
