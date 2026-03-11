# Tabby

> Self-hosted AI coding assistant — an open-source, on-premises alternative to GitHub Copilot.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://tabbyml.com)
- [GitHub Repository](https://github.com/TabbyML/tabby)

## Install

### macOS
```bash
brew install tabbyml/tabby/tabby
tabby serve --device metal --model StarCoder-1B
```

### Linux / Windows (Docker)
```bash
docker run -it --gpus all -p 8080:8080 -v $HOME/.tabby:/data \
  tabbyml/tabby serve --model StarCoder-1B --device cuda
```

For CPU-only (no GPU):
```bash
docker run -it -p 8080:8080 -v $HOME/.tabby:/data \
  tabbyml/tabby serve --model StarCoder-1B --device cpu
```

Pre-built binaries for Windows and Linux are also available on the [releases page](https://github.com/TabbyML/tabby/releases).

## Pricing
100% free when self-hosted. Open source (Apache 2.0). No usage limits, no external API calls required — all inference runs locally.

## Alternatives
- [Continue](continue.md)
- [Ollama](ollama.md)
