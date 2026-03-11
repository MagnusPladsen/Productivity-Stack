# atuin

> Replaces shell history with a SQLite database, adds fuzzy search, and supports optional encrypted cross-machine sync.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://atuin.sh/)
- [GitHub Repository](https://github.com/atuinsh/atuin) ⭐ 28.6k

## Pricing

Atuin is fully open source and free to self-host. The managed sync server (atuin.sh) is free for personal use with unlimited history sync. A paid "Atuin Plus" tier is available for teams and additional features — check the website for current pricing.

## Install

### macOS
```bash
brew install atuin
```

### Linux
```bash
# Universal install script (recommended):
curl --proto '=https' --tlsv1.2 -LsSf https://setup.atuin.sh | sh

# Arch Linux
sudo pacman -S atuin
```

### Windows
```bash
winget install -e Atuinsh.Atuin
```

## Setup

Add the shell plugin after installing:

```bash
# Bash (~/.bashrc)
eval "$(atuin init bash)"

# Zsh (~/.zshrc)
eval "$(atuin init zsh)"

# Fish (~/.config/fish/config.fish)
atuin init fish | source
```

## Alternatives
- [fzf](fzf.md)
