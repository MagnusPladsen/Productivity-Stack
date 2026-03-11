# Pencil

> AI-native frontend design tool that embeds a vector canvas directly in your IDE. Turn prompts into editable visual designs and export production-ready React, HTML, or CSS — with full MCP support.

**Platforms:** VS Code / Cursor extension + macOS app

**Pricing:** Free during early access. AI features require Claude Code (paid subscription, ~$20/month) or Anthropic API credits.

## Links
- [Official Website](https://pencil.dev)
- [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=highagency.pencildev)
- [Documentation](https://docs.pencil.dev)

## Install

### VS Code / Cursor

Search for **Pencil** in the VS Code or Cursor extension marketplace, or install from the command line:

```bash
code --install-extension highagency.pencildev
```

After installation, authenticate with the Claude Code CLI to enable AI features.

### macOS App

Download the desktop app from [pencil.dev](https://pencil.dev).

## Notes

- Design files are stored as version-controlled `.pen` (JSON-based) files in your Git repository.
- Supports importing designs from Figma.
- Exposes an MCP server for use with Claude Code and other AI agents.

## Alternatives
- [Cursor](cursor.md)
- [Windsurf](windsurf.md)
