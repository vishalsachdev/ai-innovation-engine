# Alternatives Analysis — Tool Stack Comparison

**Date:** 2026-03-29

## Recommendation Summary

| Layer | Our Pick | Best Alternative | Decision |
|---|---|---|---|
| Org simulation | **Paperclip** | CrewAI (47K stars) | Keep Paperclip — only one with budgets, governance, audit trails, company import |
| Skills framework | **gstack** + anthropics/skills | skills.sh, awesome-cursorrules | Use both — gstack for sprint workflow, skills.sh for cross-agent publishing |
| Agent backend | **Hermes Agent** | LibreChat (35K, MIT, Azure AD) | Use both — LibreChat as student frontend (SSO), Hermes as skill execution backend |
| Research platform | **ResearchChatAI** | Typebot (A/B testing, visual builder) | Use both — ResearchChatAI for conversation experiments, Typebot for structured surveys |

---

## Category 1: Agent Orchestration (vs. Paperclip)

| | CrewAI | LangGraph | AutoGen/AG2 | **Paperclip** |
|---|---|---|---|---|
| Stars | 47K | 28K | 56K/4K | 39K |
| Metaphor | Role-based teams | Graph workflows | Conversational groups | Full company |
| Budgets | No | No | No | **Yes (per-agent, hard stop)** |
| Governance | No | No | No | **Yes (approval gates, audit)** |
| Org charts | No | No | No | **Yes (reportsTo, SVG)** |
| Company import | No | No | No | **Yes (agentcompanies/v1)** |
| Teaching fit | Good (roles) | Advanced CS | Uncertain (MS transition) | **Best (org design)** |

**Verdict:** Paperclip is irreplaceable for teaching org design, budgeting, and governance. CrewAI good for quick demos.

## Category 2: AI Skills (vs. gstack)

| | anthropics/skills | skills.sh | awesome-cursorrules |
|---|---|---|---|
| Stars | 106K | npm ecosystem | 39K |
| Format | SKILL.md (official) | SKILL.md (universal) | .cursorrules (Cursor-only) |
| Sprint workflow | No | No | No |
| YC-style skills | No | No | No |

**Verdict:** gstack is unique (no alternative has `/office-hours`, `/plan-ceo-review`, `/retro`). Publish Gies customs via skills.sh for cross-agent compat.

## Category 3: Agent Backend (vs. Hermes)

| | Open WebUI | Dify | LobeChat | **LibreChat** |
|---|---|---|---|---|
| Stars | 129K | 135K | 74K | 35K |
| License | MIT | Apache (multi-tenant restricted) | PolyForm | **MIT** |
| SSO | Basic RBAC | Enterprise only | Multi-user | **Azure AD, SAML, OAuth2** |
| Moderation | Basic | Yes | Limited | **Full (Harvard a11y)** |
| MCP | Limited | Yes | Yes | **Yes** |

**Verdict:** LibreChat for student-facing (Azure AD = Illinois SSO, MIT license, accessibility). Hermes for skill execution backend.

## Category 4: Research (vs. ResearchChatAI)

| | Botpress | Rasa | **Typebot** |
|---|---|---|---|
| Stars | 15K | 21K | 10K |
| A/B testing | Via flow variants | No | **Built-in** |
| Self-host | Docker or cloud | Kubernetes (heavy) | Docker |
| IRB features | Analytics + logging | Full conversation logs | Webhook + data collection |

**Verdict:** ResearchChatAI for conversation experiments (field-level encryption, condition management). Typebot for structured A/B surveys.
