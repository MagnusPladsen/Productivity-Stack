# Windsurf

> AI-first code editor (VS Code fork) with flow-based agentic AI via the Cascade agent.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://windsurf.com)

## Install

### macOS
Download the `.dmg` from [windsurf.com/download/editor](https://windsurf.com/download/editor) and drag to Applications.

### Linux (Debian/Ubuntu)
```bash
curl -fsSL "https://windsurf-stable.codeiumdata.com/wVxQEIWkwPUEAGf3/windsurf.gpg" \
  | sudo gpg --dearmor -o /usr/share/keyrings/windsurf-stable-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/windsurf-stable-archive-keyring.gpg arch=amd64] \
  https://windsurf-stable.codeiumdata.com/wVxQEIWkwPUEAGf3/apt stable main" \
  | sudo tee /etc/apt/sources.list.d/windsurf.list > /dev/null

sudo apt update && sudo apt install windsurf
```

An AppImage is also available for other Linux distributions from [windsurf.com/download/editor](https://windsurf.com/download/editor).

### Windows
Download the `.exe` installer from [windsurf.com/download/editor](https://windsurf.com/download/editor) and run it.

## Pricing
Free tier includes: 25 prompt credits/month, unlimited Tab autocomplete (fast), access to the SWE-1 Lite model, and 1 app deployment/day. Paid plans start at $15/month (Pro) for unlimited Cascade interactions and premium model access.

## Alternatives
- [Cursor](cursor.md)
- [Antigravity](antigravity.md)
