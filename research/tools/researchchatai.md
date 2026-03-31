# ResearchChatAI — Technical Analysis

**Repo:** [ResearchChatAI/ResearchChatAI](https://github.com/ResearchChatAI/ResearchChatAI) | **License:** MIT
**Origin:** Universiteit Maastricht, VU Amsterdam, WHU, Babson College

## What It Is

Open-source platform for running controlled chatbot-based research studies. Researcher configures an AI agent through a 5-step wizard, distributes a link, participants chat with the chatbot, conversations are collected with field-level encryption.

## Tech Stack
- PHP (81.1%), JavaScript (16.6%), MySQL, Node.js (stream proxy)
- AES-256-CBC symmetric + RSA-2048 hybrid encryption
- Custom connector system (OpenAI, Anthropic, Google, Mistral, OpenRouter)

## Research Features

| Feature | Application |
|---|---|
| **Experimental conditions** | Multiple treatment arms with per-condition AI name, instructions, avatar, colors |
| **Embedded variables** | `{{variableName}}` from URL params (studentID, condition, section) |
| **Conversation export** | CSV of all conversations + submissions |
| **Field-level encryption** | IRB-compliant (AES-256-CBC + RSA-2048) |
| **Custom connectors** | Point at Hermes backend instead of direct provider |
| **Reasoning display** | Collapsible chain-of-thought panel for models with reasoning |

## Limitations
- No multi-user collaboration (single researcher per study)
- No public API or embedding SDK
- No document/citation handling (pure conversation platform)

## Integration Path

ResearchChatAI's custom connector → Hermes's OpenAI-compatible API. Students interact with ResearchChatAI frontend (controlled experiment UI), ResearchChatAI proxies to Hermes (real skills + memory), researcher gets structured, encrypted data with condition labels.
