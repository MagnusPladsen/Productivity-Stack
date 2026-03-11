# Open WebUI

> User-friendly web interface for running AI models locally, supporting Ollama and OpenAI-compatible APIs.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://openwebui.com/)
- [GitHub Repository](https://github.com/open-webui/open-webui)
- [Documentation](https://docs.openwebui.com/)

## Install

### macOS / Linux / Windows (via pip)

Requires Python 3.11+.

```bash
pip install open-webui
open-webui serve
```

Access at http://localhost:8080.

### macOS / Linux / Windows (via Docker)

```bash
docker run -d -p 3000:8080 \
  -v open-webui:/app/backend/data \
  --name open-webui \
  --restart always \
  ghcr.io/open-webui/open-webui:main
```

Access at http://localhost:3000.

## Alternatives
- [Open Router](open-router.md)
