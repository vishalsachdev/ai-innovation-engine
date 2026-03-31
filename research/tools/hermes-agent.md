# Hermes Agent — Technical Analysis

**Repo:** [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | **Stars:** ~16.6K | **License:** MIT
**Author:** Nous Research

## What It Is

Self-improving AI agent framework. Core differentiator: a learning loop where the agent creates, refines, and reuses skills across sessions, plus persistent user modeling and cross-session search.

## Tech Stack
- Python 3.11+ (92.3%), uv package manager
- CLI: prompt_toolkit + Rich + Fire
- LLM: openai SDK, anthropic SDK (direct adapters)
- Gateway: 13 platform adapters (Telegram, Discord, Slack, WhatsApp, Matrix, Signal, etc.)
- API: OpenAI-compatible HTTP server (compatible with Open WebUI, LobeChat, LibreChat, etc.)

## Key Features for Shared Rails

| Feature | Infrastructure Application |
|---|---|
| **Profiles** | Each course/project gets isolated config, keys, memory, skills, sessions |
| **Skill system** | Self-registering skills in `~/.hermes/skills/`. Agent creates skills after successful tasks |
| **Plugin hooks** | `pre_tool_call`, `post_tool_call`, `pre_llm_call`, `post_llm_call` = logging, guardrails, research instrumentation |
| **OpenAI-compatible API** | Any frontend plugs in without rewriting |
| **MCP server** | Claude Code / Cursor can orchestrate Hermes agents |
| **Terminal backends** | Docker (local), Modal (serverless), SSH, Singularity (HPC) |
| **Skills Hub** | Federated discovery from 7+ sources: bundled, GitHub, skills.sh, ClawHub, LobeHub |

## Multi-Tenancy

Session isolation via SQLite: keyed by platform + chat_id, optionally by thread_id and user_id. Profiles provide full instance-level isolation. Not built for SaaS-scale multi-tenancy — better paired with LibreChat for the student-facing layer.

## Recommendation

Use Hermes as the **skill execution backend** (profiles per course, rich skill system), but pair with **LibreChat** for the student-facing frontend (Azure AD SSO for Illinois, MIT license, moderation, accessibility).
