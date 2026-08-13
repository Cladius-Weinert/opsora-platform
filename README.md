# Opsora AI Platform v2

**One Terminal. Every AI Provider. Zero Vendor Lock-in.**

Multi-provider AI gateway with intelligent fallback, real-time cost tracking, and streaming.

## Features

- **Landing Page** — Hero, providers grid, features, pricing, agent playground
- **Agent Chat** — Multi-model chat with streaming, cost tracking, typing indicators
- **Dashboard** — Real-time analytics, provider health, model distribution
- **Dark Theme** — Cyber-teal aesthetic with glassmorphism, gradient orbs, noise textures

## Architecture

```
Landing Page → Agent Chat → Dashboard
         ↓
Cloudflare Worker Gateway
  ├── NVIDIA NIM (primary)
  ├── Alibaba DashScope (fallback)
  ├── OpenAI / AWS / Google / Meta
  └── Auth + Rate Limiting + Analytics
         ↓
ADP Agent Platform → GitHub Repos → CLI → API → Docs
```

## Links

- [CLI](https://github.com/Cladius-Weinert/opsora-cli)
- [Agent API](https://github.com/Cladius-Weinert/opsora-agent-api)
- [Gateway](https://opsora-gateway.opsora-ai.workers.dev)
- [API Docs](https://github.com/Cladius-Weinert/opsora-api-docs)