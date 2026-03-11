# OpenRouter

> Unified API gateway and web interface for routing requests across dozens of AI models from different providers.

**Platforms:** Web

## Links
- [Official Website](https://openrouter.ai/)

## Install

OpenRouter is a web-based service — no installation required. Sign up at https://openrouter.ai/ and use the API or web chat interface directly.

To use the OpenRouter API in your own projects:

```bash
# Example: call any model via the OpenRouter API
curl https://openrouter.ai/api/v1/chat/completions \
  -H "Authorization: Bearer $OPENROUTER_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"model": "openai/gpt-4o", "messages": [{"role": "user", "content": "Hello"}]}'
```

## Alternatives
- [Open WebUI](open-webui.md)
