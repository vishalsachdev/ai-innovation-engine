# LibreChat — Technical Analysis

**Repo:** [danny-avila/LibreChat](https://github.com/danny-avila/LibreChat) | **Stars:** ~35K | **License:** MIT
**Author:** Danny Avila + community

## What It Is

Self-hosted AI chat platform that unifies all major AI providers (OpenAI, Anthropic, Google, Azure, AWS, Mistral, etc.) behind a single, privacy-focused interface. Features agents, MCP support, artifacts, code interpreter, conversation search, and enterprise-ready multi-user auth.

## Tech Stack
- Node.js + Express backend, React + Vite frontend
- MongoDB (Mongoose ODM) for data storage
- Docker Compose for production deployment (NGINX/Traefik reverse proxy)
- Also deployable on Railway, Zeabur, Sealos, or bare Node.js

## Key Features for Student Frontend

| Feature | Infrastructure Application |
|---|---|
| **Azure AD / Entra ID SSO** | Illinois university SSO via OIDC — also supports SAML, LDAP, OAuth2, Okta, Keycloak |
| **MCP support** | Connect to Hermes backend, Canvas MCP, custom tools via Model Context Protocol |
| **Agents** | Custom agent definitions with tool access, configurable per use case |
| **Code Interpreter** | Sandboxed code execution — safe for student experimentation |
| **Artifacts** | Rich output rendering (code, diagrams, documents) |
| **Multi-user auth** | User registration, 2FA, role-based access, session management |
| **Moderation system** | Automated scoring: tracks violations, rate limits logins/messages, IP + user-level bans |
| **Conversation search** | Full-text search across chat history |
| **Presets** | Pre-configured model/system-prompt combos — one per course or assignment |
| **WCAG accessibility** | Screen reader support, keyboard navigation, focus management, contrast ratios |

## SSO / Authentication Details

- Azure Entra ID tokens can be reused for session management (Azure refresh tokens instead of internal session tokens)
- Microsoft Graph API integration for people/group search (admin consent may be required — same Illinois tenant policy that blocked MS365 MCP)
- OIDC integration with any compliant provider (Okta, Keycloak, Auth0, etc.)
- SAML and LDAP also supported as alternatives

## Moderation & Safety

- **Violation scoring**: Users accumulate scores for excessive logins, registrations, or messaging
- **Auto-banning**: Temporary bans at configurable threshold (user + IP)
- **Rate limiting**: Per-IP and per-user message frequency, concurrent message limits
- **Brute force protection**: Login attempt and registration throttling
- **Data isolation**: Code interpreter runs in sandboxes; all data stays on-server unless external services configured

## Education Fit

- Multilingual AI tutor capabilities (explain concepts, run code, visualize)
- Multimodal lessons with code execution, image illustration, speech interaction
- Presets system maps well to per-course configurations
- Self-hosted = full data sovereignty (important for IRB compliance)
- Docker deployment = manageable for university IT

## Integration Path

LibreChat serves as the **student-facing frontend layer**:
1. Students authenticate via Illinois SSO (Azure Entra ID → OIDC)
2. LibreChat connects to Hermes Agent backend via MCP or OpenAI-compatible API
3. Hermes provides skill execution, persistent memory, user profiles per course
4. Course presets in LibreChat map to Hermes profiles
5. Conversation data flows to ResearchChatAI for research instrumentation

## Why LibreChat Over Alternatives

| | Open WebUI (129K) | Dify (135K) | LobeChat (74K) | **LibreChat (35K)** |
|---|---|---|---|---|
| License | MIT | Apache (multi-tenant restricted) | PolyForm (restrictive) | **MIT** |
| SSO | Basic RBAC | Enterprise only | Multi-user | **Azure AD, SAML, LDAP, OAuth2** |
| Moderation | Basic | Yes | Limited | **Full (scoring, bans, rate limits)** |
| MCP | Limited | Yes | Yes | **Yes (agent-level configuration)** |
| Accessibility | Unknown | Unknown | Unknown | **WCAG improvements (screen reader, keyboard, contrast)** |
| Code execution | Yes | Yes | No | **Yes (sandboxed)** |

Open WebUI has more stars but lacks enterprise SSO. Dify restricts multi-tenant under Apache. LobeChat's PolyForm license is problematic for university use. LibreChat's MIT license + full Azure AD SSO + moderation makes it the best fit for a university deployment.
