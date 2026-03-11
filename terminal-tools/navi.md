# navi

> Interactive CLI cheatsheet tool — browse, search, and execute shell snippets with fuzzy search, with support for community cheatsheet repos.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://github.com/denisidoro/navi)
- [GitHub Repository](https://github.com/denisidoro/navi) ⭐ 16.8k

## Install

### macOS
```bash
brew install navi
```

### Linux
```bash
# Cargo (requires Rust)
cargo install navi

# Arch Linux (AUR)
yay -S navi
```

### Windows
```bash
# Cargo (requires Rust)
cargo install navi
```

## Setup

After installing, run `navi` to fetch community cheatsheets on first launch, or add your own:

```bash
# Browse and execute cheatsheets interactively
navi

# Use as a shell widget (Ctrl+G) by adding to ~/.zshrc or ~/.bashrc:
eval "$(navi widget zsh)"
```

## Alternatives
- [tldr](tldr.md)
- [fzf](fzf.md)
