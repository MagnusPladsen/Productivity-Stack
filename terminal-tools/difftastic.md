# difftastic

> A structural diff tool that compares files based on their syntax, not line-by-line.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://difftastic.wilfred.me.uk/)
- [GitHub Repository](https://github.com/Wilfred/difftastic) ⭐ 24.4k

## Install

### macOS
```bash
brew install difftastic
```

### Linux
```bash
# Cargo (recommended)
cargo install --locked difftastic

# Arch Linux
sudo pacman -S difftastic

# Fedora
sudo dnf install difftastic

# Snap
sudo snap install difftastic
```

### Windows
```bash
winget install Wilfred.difftastic
```

## Overview

difftastic understands the grammar of your code. Instead of comparing raw text line-by-line, it parses both files into ASTs and diffs the structure. The result is that whitespace-only changes and reformatting don't produce noisy diffs, and moved code is shown clearly.

Supports 30+ languages including Rust, Python, TypeScript, Go, C, Java, and more. Falls back to line-oriented diffing for unsupported file types.

```bash
# Use as a standalone diff
difft old.js new.js

# Use with git
GIT_EXTERNAL_DIFF=difft git diff
GIT_EXTERNAL_DIFF=difft git log -p --ext-diff

# Configure git globally
git config --global diff.external difft
```

## Alternatives
- [delta](delta.md)
