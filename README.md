## Hey, I'm Marley 👋

**IT manager who builds.** By day I run enterprise IT for a 22-site, ~3,900-employee company: three years in IT, promoted from technician to manager in 13 months, on twelve years of retail operations before that. The rest of the time I build the systems that automate the work: an AI-native helpdesk, an LLM orchestration platform, and a self-hosted Kubernetes fleet of production agents. Everything below runs on infrastructure I operate.

### What I've shipped

🎫 **AI-native helpdesk, in production** — architected the middleware and omnichannel intake for a staged move from a commercial ITSM suite to open-source Zammad plus custom AI: AI ticket triage and routing, auto-assignment by store, vendor email pipelines, a voice-to-ticket path, an after-hours AI receptionist with emergency SMS paging, and knowledge-base-grounded answers. ~31K tickets migrated; the legacy system stays the system of record until cutover. The open-source starter for the same pattern is **[zammad-ai-starter](https://github.com/saltxd/zammad-ai-starter)**: Zammad and an AI triage worker in one `docker compose up`, routed by Claude or a local Ollama model.

🏷️ **[ttb-label-check](https://github.com/saltxd/ttb-label-check)** — verifies alcohol-label images against COLA application data (brand, ABV, the 27 CFR Part 16 health warning). FastAPI + Tesseract/OpenCV, local-first with optional vision-model assist, TDD from the first commit, and an OCR retry ladder measured against a hard-image set. Live at [ttb.chainward.ai](https://ttb.chainward.ai), two replicas on my own cluster.

🤖 **GPT-OS** — a self-hosted LLM orchestration platform (~44K lines of Python, 630+ tests, CI-gated, 10-service stack, in production since 2025): multi-provider routing with fallback, RAG with automatic memory capture, MCP tool use behind a hardened sandbox, and a shared desk where named agents work in front of the operator. The repo is private because it is wired into my infrastructure; the [architecture writeup](https://gist.github.com/saltxd/cee5ee1a312292b911e64bbf4e8709bf) is public.

⛓️ **[chainward](https://github.com/saltxd/chainward)** — an automated, adversarially verified on-chain investigation engine for AI agents on Base: TypeScript monorepo, 16-worker queue indexer, TimescaleDB, and a verifier gauntlet that re-checks every numeric claim before anything publishes. Reads from a self-hosted Base node.

🏗️ **Homelab platform** — 4-node Proxmox / K3s HA cluster (3 control planes + etcd), Longhorn storage, Prometheus/Grafana/Alertmanager, GitOps deploys, plus a fleet of scheduled autonomous LLM agents with least-privilege MCP access and OpenTelemetry tracing to a self-hosted Arize Phoenix.

🔥 **[streak-tracker](https://github.com/saltxd/streak-tracker)** — a small, finished thing: a macOS menu-bar streak tracker in SwiftUI, released as a prebuilt universal app.

### Tech stack

```
Languages         Python · TypeScript · SQL · Bash · PowerShell · Swift
Platform          Kubernetes (K3s HA) · Docker · Proxmox · GitHub Actions · GitOps · Cloudflare Tunnel
Backend / Data    FastAPI · Hono · BullMQ · PostgreSQL/TimescaleDB · Redis
Applied AI        Claude / OpenAI / Ollama · RAG · MCP · agent orchestration · evals & tracing
Enterprise IT     Microsoft 365 · Entra ID · Active Directory · ManageEngine · Zammad · Fortinet
```

### Writing

I write about AI-native, self-hosted IT automation: running LLM agents in production on infrastructure you own, safely and cheaply.

- [I replaced 1,000 lines of Python with a 500-word prompt](https://dev.to/saltxd/i-replaced-1000-lines-of-python-with-a-500-word-prompt-29ao)
