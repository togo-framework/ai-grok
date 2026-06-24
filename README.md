# ai-grok

xAI Grok driver for the togo `ai` plugin — a unified LLM interface (chat + embeddings) for togo apps.

## Install
```bash
togo install togo-framework/ai-grok
```

## Configure
Set `AI_DRIVER=grok` and:
```env
XAI_API_KEY=...
# optional: XAI_BASE_URL=https://api.x.ai/v1
```

Then the `ai` plugin routes `Chat`/`Embed` through xAI Grok. Token usage is reported via `ai.Usage` (for the billing plugin).

MIT © ToGO
