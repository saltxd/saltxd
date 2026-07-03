## Hey, I'm Marley 👋

**IT Automation & Platform Engineer.** 13 years in operations and enterprise IT — I lead an IT team by day and build the systems that automate the work: AI-powered helpdesk automation, LLM orchestration platforms, and self-hosted Kubernetes infrastructure.

### What I've shipped

🎫 **Replaced a commercial ITSM in production** — architected the middleware and omnichannel intake for a move from a commercial helpdesk suite to open-source + custom AI for a ~3,900-employee company: AI ticket triage/routing, a voice→ticket pipeline, an AI receptionist, and knowledge-base-grounded answers. Migrated ~31K tickets and retired the license.

🤖 **GPT-OS** — a self-hosted LLM orchestration platform (~31K lines of Python, 433 tests, CI-gated, 10-service stack, in production since 2025): multi-provider routing with fallback, RAG with automatic memory capture, and MCP tool use behind a hardened sandbox. The repo is private because it's wired into my personal infrastructure — [full architecture writeup here](https://gist.github.com/saltxd/cee5ee1a312292b911e64bbf4e8709bf).

⛓️ **[chainward](https://github.com/saltxd/chainward)** — an automated, adversarially-verified on-chain investigation engine for AI agents on Base: TypeScript monorepo, 16-worker queue indexer, TimescaleDB, and a verifier gauntlet that re-checks every numeric claim before anything publishes. Reads from a self-hosted Base node.

🏗️ **Homelab platform** — 4-node Proxmox / K3s HA cluster (3 control planes + etcd), Longhorn storage, Prometheus/Grafana/Alertmanager, GitOps deploys — plus a fleet of scheduled autonomous LLM agents with least-privilege MCP access and OpenTelemetry tracing to a self-hosted Arize Phoenix.

🔥 **[streak-tracker](https://github.com/saltxd/streak-tracker)** — a small, finished thing: a macOS menu-bar streak tracker in SwiftUI, released with a prebuilt universal app.

### Tech stack

```
Languages         Python · TypeScript · SQL · Bash · PowerShell
Platform          Kubernetes (K3s HA) · Docker · Proxmox · GitHub Actions · GitOps
Backend / Data    FastAPI · Hono · BullMQ · PostgreSQL/TimescaleDB · Redis
Applied AI        Claude / OpenAI / Ollama · RAG · MCP · agent orchestration · evals & tracing
Enterprise IT     Microsoft 365 · Active Directory · ManageEngine · Fortinet
```

### Writing

I write about **AI-native, self-hosted IT automation** — running LLM agents in production on infrastructure you own, safely and cheaply.
