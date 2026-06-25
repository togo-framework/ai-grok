# ai-grok — documentation

xAI Grok LLM driver for togo ai

## Overview

Package grok is a xAI Grok driver for togo ai (OpenAI-compatible API).
Blank-import it and set AI_DRIVER=grok + XAI_API_KEY.

## Install

```bash
togo install togo-framework/ai-grok
```

Set `AI_DRIVER=grok`.

## Configuration

Environment variables read by this plugin (extracted from the source — see the gateway/provider docs for each value):

| Env var |
|---|
| `XAI_BASE_URL` |

## Usage

```go
provider := ai.FromKernel(k)
resp, err := provider.Chat(ctx, []ai.Message{{Role: "user", Content: "Hello"}}, ai.Options{})
// streaming + provider.Embed(ctx, texts) for vectors; resp.Usage carries token counts
```

## Links

- Marketplace: https://to-go.dev/marketplace
- Source: https://github.com/togo-framework/ai-grok
- Full README: ../README.md
