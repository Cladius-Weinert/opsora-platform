# Opsora AI Platform v2

**One API. Every model. Zero lock-in.**

Multi-provider AI gateway. Route to NVIDIA NIM, Alibaba DashScope, OpenAI, AWS Bedrock, Meta Llama, Google Gemini. Intelligent fallback, real-time cost tracking, edge deployment.

## 🚀 Deployment Status

| Component | Status | URL |
|---|---|---|
| **AI Gateway** | ✅ **Live** | `https://opsora-gateway.opsora-ai.workers.dev` |
| **EdgeOne Pages** | ✅ **Live** | `https://mcp.edgeone.site/share/r6zJP900KH9WucWcvpDyV` |
| **GitHub Repo** | ✅ **Live** | `https://github.com/Cladius-Weinert/opsora-platform` |
| **GitHub Pages** | ⏳ Enable in Settings | `https://cladius-weinert.github.io/opsora-platform` |

## 🏗️ Pages

- **Landing** → `index.html` — Hero, providers, features, pricing, playground, dashboard
- **Agent Chat** → `agent.html` — Full-screen chat with sidebar navigation
- **Dashboard** → `dashboard.html` — Stats, charts, provider health

## ⚡ Gateway API

The Opsora Gateway supports OpenAI-compatible API calls:

```bash
curl https://opsora-gateway.opsora-ai.workers.dev/v1/chat/completions \
  -H "Content-Type: application/json" \
  -d '{
    "model": "nvidia/nemotron-mini-4b-instruct",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
```

### Available Models

| Model | Provider | Type |
|---|---|---|
| `meta/llama-3.1-8b-instruct` | NVIDIA | General |
| `meta/llama-3.1-70b-instruct` | NVIDIA | Large |
| `nvidia/nemotron-mini-4b-instruct` | NVIDIA | Fast |
| `nvidia/nemotron-3-super-120b-a12b` | NVIDIA | Max |
| `deepseek-ai/deepseek-v4-flash` | NVIDIA | (EOL) |
| `qwen-turbo` | DashScope | Fast |
| `qwen-plus` | DashScope | Balanced |
| `qwen-max` | DashScope | Max |
| `qwen3-coder-flash` | DashScope | Code |

## 🛠️ Tech Stack

- **Frontend**: Vanilla HTML/CSS/JS — Instrument Serif + Rubik + JetBrains Mono
- **Gateway**: Cloudflare Workers (Edge)
- **Backend**: FastAPI / Python (opsora-agent-api)
- **CLI**: Python (opsora-cli)
- **Deployment**: GitHub Pages / EdgeOne / Fly.io / Render

## 📋 Getting Started

1. **Enable GitHub Pages**: Go to Repo Settings → Pages → Source: `main` → `/` → Save
2. **Deploy Agent API**: Use `fly launch` or `docker compose up` in opsora-agent-api
3. **Get API Key**: Register at `https://opsora-gateway.opsora-ai.workers.dev/auth/register`

## 📚 Repos

- [Opsora CLI](https://github.com/Cladius-Weinert/opsora-cli)
- [Opsora Agent API](https://github.com/Cladius-Weinert/opsora-agent-api)
- [Opsora API Docs](https://github.com/Cladius-Weinert/opsora-api-docs)
- [Opsora Multi-Region](https://github.com/Cladius-Weinert/opsora-multi-region)
- [Opsora Landing](https://github.com/Cladius-Weinert/opsora-landing)