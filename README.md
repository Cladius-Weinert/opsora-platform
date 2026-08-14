# Opsora AI Platform v2

**One API. Every model. Zero lock-in.**

Multi-provider AI gateway. Route to NVIDIA NIM, Alibaba DashScope, OpenAI, AWS Bedrock, Meta Llama, Google Gemini. Intelligent fallback, real-time cost tracking, edge deployment.

## 🚀 Deployment Status

| Component | Status | URL |
|---|---|---|
| **AI Gateway** | ✅ **Live** | `https://opsora-gateway.opsora-ai.workers.dev` |
| **EdgeOne Pages** | ✅ **Live** | `https://mcp.edgeone.site/share/r6zJP900KH9WucWcvpDyV` |
| **GitHub Repo** | ✅ **Live** | `https://github.com/Cladius-Weinert/opsora-platform` |
| **ADP App** | ✅ **Created** | App ID: `2088166720708938496` |
| **GitHub Pages** | ⏳ Enable in Settings | `https://cladius-weinert.github.io/opsora-platform` |

## 🏗️ Pages

- **Landing** → `index.html` — Hero, 6 providers, 9 features, 3-tier pricing, playground, analytics
- **Agent Chat** → `agent.html` — Full-screen chat with sidebar, typing indicators, cost tracking
- **Dashboard** → `dashboard.html` — 4 stat cards, daily bar chart, provider health table

## 🤖 ADP App

An ADP application has been created for Opsora AI:

- **App ID**: `2088166720708938496`
- **Model**: DeepSeek V4 Flash
- **Agent Prompt**: Opsora AI multi-provider assistant
- **Features**: Knowledge base retrieval, model routing
- **Management URL**: `https://adp.tencentcloud.com/adp?spaceId=default_space#/app/knowledge/app-config?appid=2088166720708938496`

## ⚡ Gateway API

```bash
curl https://opsora-gateway.opsora-ai.workers.dev/v1/chat/completions \
  -H "Content-Type: application/json" \
  -d '{"model":"nvidia/nemotron-mini-4b-instruct","messages":[{"role":"user","content":"Hello!"}]}'
```

## 🛠️ Tech Stack

- **Frontend**: Vanilla HTML/CSS/JS — Instrument Serif + Rubik + JetBrains Mono
- **Gateway**: Cloudflare Workers (Edge)
- **ADP**: Tencent Cloud Agent Development Platform
- **Backend**: FastAPI / Python (opsora-agent-api)
- **CLI**: Python (opsora-cli)
- **Deployment**: GitHub Pages / EdgeOne / Fly.io / Render

## 📚 Repos

- [Opsora CLI](https://github.com/Cladius-Weinert/opsora-cli)
- [Opsora Agent API](https://github.com/Cladius-Weinert/opsora-agent-api)
- [Opsora API Docs](https://github.com/Cladius-Weinert/opsora-api-docs)
- [Opsora Multi-Region](https://github.com/Cladius-Weinert/opsora-multi-region)
- [Opsora Landing](https://github.com/Cladius-Weinert/opsora-landing)