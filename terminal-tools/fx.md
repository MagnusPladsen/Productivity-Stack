# fx

> Interactive terminal JSON/YAML/TOML viewer and processor.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://fx.wtf/)
- [GitHub Repository](https://github.com/antonmedv/fx) ⭐ 20.3k

## Install

### macOS
```bash
brew install fx
```

### Linux
```bash
# npm (cross-platform)
npm install -g fx

# Download binary from releases
# https://github.com/antonmedv/fx/releases
```

### Windows
```bash
npm install -g fx
```

## Overview

fx is a terminal JSON viewer and processor. In interactive mode, it renders JSON as a collapsible tree you can navigate with the keyboard, search, and filter. In non-interactive mode, it works as a lightweight `jq` alternative using JavaScript expressions.

```bash
# Interactive viewer
curl https://api.github.com/repos/antonmedv/fx | fx

# Extract a field (JS expression)
echo '{"name":"alice"}' | fx .name

# Filter an array
cat data.json | fx '.users.filter(u => u.active)'

# Works with YAML and TOML too
cat config.yaml | fx
```

## Alternatives
- [jq](jq.md)
- [gron](gron.md)
