# starship

> Blazing-fast, cross-shell prompt written in Rust — minimal, customizable, works with any shell.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://starship.rs/)
- [GitHub Repository](https://github.com/starship/starship) ⭐ 54.8k

## Install

### macOS
```bash
brew install starship
```

### Linux
```bash
sudo apt install starship
```

### Windows
```bash
winget install --id Starship.Starship
```

## Setup

Add the init line to your shell config after installing:

```bash
# Bash (~/.bashrc)
eval "$(starship init bash)"

# Zsh (~/.zshrc)
eval "$(starship init zsh)"

# Fish (~/.config/fish/config.fish)
starship init fish | source

# PowerShell ($PROFILE)
Invoke-Expression (&starship init powershell)
```

## Alternatives
- [oh-my-zsh](oh-my-zsh.md)
