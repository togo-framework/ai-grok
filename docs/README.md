# ai-grok — documentation

  <img src=".github/assets/togo-mark.svg" alt="togo" height="64" />

## Overview

Package grok is a xAI Grok driver for togo ai (OpenAI-compatible API).
Blank-import it and set AI_DRIVER=grok + XAI_API_KEY.

## Install

```bash
togo install togo-framework/ai-grok
```

Set `AI_DRIVER=grok`.

## Configuration

Environment variables read by this plugin (extracted from the source):

| Env var | Notes |
|---|---|
| `G` | _see provider docs_ |
| `XAI_BASE_URL` | _see provider docs_ |

## Usage

```go
provider := ai.FromKernel(k)
resp, err := provider.Chat(ctx, []ai.Message{{Role: "user", Content: "Hello"}}, ai.Options{})
// streaming + provider.Embed(ctx, texts) for vectors; resp.Usage carries token counts
```

## Links

- Marketplace: https://to-go.dev/marketplace
- Source: https://github.com/togo-framework/ai-grok
- README: ../README.md
