# Paperclip — Technical Analysis

**Repo:** [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | **Stars:** ~39K | **License:** MIT
**Tagline:** "If OpenClaw is an employee, Paperclip is the company"

## What It Is

Self-hosted orchestration platform for "zero-human companies." Coordinates multiple AI agents into a company structure with org charts, budgets, governance, goal alignment, and a ticket system. Not an agent framework — assumes you already have agents and provides the organizational layer.

## Tech Stack
- TypeScript (entire codebase), Node.js 20+, pnpm monorepo
- Server: Custom Node.js with Express-style routes
- DB: Embedded PostgreSQL (PGlite) or BYO Postgres, Drizzle ORM
- UI: React + Vite + shadcn/ui
- Testing: Vitest + Playwright
- 10 agent adapters: claude_local, codex_local, cursor, gemini_local, opencode_local, pi_local, openclaw_gateway, hermes, process, http

## Teaching-Critical Features

| Feature | Teaching Application |
|---|---|
| **Org charts** (`reportsTo` field, SVG rendering) | Students design hierarchies, compare flat vs deep |
| **Budget system** (per-agent/project/company, hard stops, soft warnings) | Resource allocation, burn rate, unit economics |
| **Governance** (approval gates, board oversight, config revisions with rollback) | Corporate governance, principal-agent problem |
| **Ticket system** (atomic checkout, status lifecycle, audit trail) | Project management, accountability |
| **Cost tracking** (per-agent, per-model, per-project, rolling windows) | Token economics, ROI analysis |
| **Company templates** (`agentcompanies/v1` spec, portable packages) | Reusable org designs, import/export |

## Company Import System

Portable company packages via `agentcompanies/v1` spec:
```
company-slug/
├── COMPANY.md
├── agents/<slug>/AGENTS.md
├── teams/<slug>/TEAM.md
├── projects/<slug>/PROJECT.md
├── tasks/<slug>/TASK.md
├── skills/<slug>/SKILL.md
└── .paperclip.yaml
```

Import: `paperclip company import <url-or-path>`
Export: Full export with secret scrubbing, collision handling, org chart PNG.

## gstack Integration
- Import shorthand: `paperclipai/companies/gstack`
- UI has gstack-specific rename logic (e.g., "gstack" + "CEO" → "gstack-CEO")
- Company creator recognizes gstack skills and routes to `claude_local` adapter

## Cloned To
`/tmp/paperclip` (shallow clone, 2026-03-29)
