# gstack — Technical Analysis

**Repo:** [garrytan/gstack](https://github.com/garrytan/gstack) | **Stars:** 55K+ | **License:** MIT
**Author:** Garry Tan, President & CEO of Y Combinator

## What It Is

Open-source Claude Code skill pack that turns the AI into a "virtual engineering team" via ~29 slash-command skills covering the full SDLC: ideation, planning, design, coding, review, QA, security, shipping, deployment, and retrospectives.

## Tech Stack
- TypeScript (79.6%), Go (18.3%)
- Bun runtime (compiled binaries, native SQLite/TypeScript/HTTP)
- Playwright (persistent Chromium daemon over CDP)
- ~58MB compiled binary for browser automation

## Key Skills (Teaching-Relevant)

| Skill | What It Does | Teaching Value |
|---|---|---|
| `/office-hours` | YC-style product diagnostic with 6 forcing questions | Idea validation, Socratic method |
| `/plan-ceo-review` | CEO-level plan review with 18 cognitive patterns (Bezos, Grove, Munger, etc.) | Strategic thinking, mental models |
| `/plan-design-review` | Rates 9 design dimensions 0-10 | Design thinking, critique |
| `/autoplan` | Chains CEO + design + eng review | Multi-stakeholder review process |
| `/qa` | Opens browser, finds bugs, fixes them, writes regression tests | QA process, quality culture |
| `/cso` | 14-phase security audit (OWASP Top 10, STRIDE) | Security/risk thinking |
| `/retro` | Data-driven retrospective from git history | Continuous improvement |
| `/ship` | Full ship workflow: tests, review, PR | Shipping discipline |

## Customization

Skills are pure Markdown (`SKILL.md` files). Entire behavior defined in prose — no compiled code for skill logic. To customize:
1. Copy any skill directory
2. Edit `SKILL.md.tmpl` or `SKILL.md` directly
3. Change YAML frontmatter + prose instructions

YC-specific content concentrated in: `ETHOS.md`, Voice section (in preamble), `/office-hours` startup mode. Can be generalized by replacing these files.

## Paperclip Integration

Paperclip's company creator explicitly mentions gstack: "gstack is built for Claude Code, so `claude_local` is appropriate." Import command: `paperclip company import paperclipai/companies/gstack`. Test cases in Paperclip's codebase confirm this is a designed pathway.

## Cloned To
`/tmp/gstack` (shallow clone, 2026-03-29)
