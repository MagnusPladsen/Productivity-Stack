# oh-my-posh

> Cross-shell prompt theme engine with hundreds of built-in themes and full customization.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://ohmyposh.dev/)
- [GitHub Repository](https://github.com/JanDeDobbeleer/oh-my-posh)

## Install

### macOS
```bash
brew install oh-my-posh
```

### Linux
```bash
brew install oh-my-posh

# Or via curl script
curl -s https://ohmyposh.dev/install.sh | bash -s
```

### Windows
```bash
winget install JanDeDobbeleer.OhMyPosh --source winget
```

## Shell Configuration

After installing, add the init line to your shell's config file:

```bash
# Bash (~/.bashrc)
eval "$(oh-my-posh init bash)"

# Zsh (~/.zshrc)
eval "$(oh-my-posh init zsh)"

# Fish (~/.config/fish/config.fish)
oh-my-posh init fish | source

# PowerShell ($PROFILE)
oh-my-posh init pwsh | Invoke-Expression
```

## Overview

oh-my-posh is a prompt engine written in Go that works identically across Bash, Zsh, Fish, PowerShell, and more. Prompts are defined in JSON/YAML/TOML config files called themes. It ships with 100+ built-in themes and supports segments for Git status, language runtimes, cloud contexts, battery, time, and much more.

```bash
# Preview all built-in themes
oh-my-posh theme print

# Use a specific theme
eval "$(oh-my-posh init zsh --config $(brew --prefix oh-my-posh)/themes/agnoster.omp.json)"

# Export current theme to customize
oh-my-posh config export --output ~/.mytheme.omp.json

# Use custom config
eval "$(oh-my-posh init zsh --config ~/.mytheme.omp.json)"
```

A Nerd Font is recommended for icon segments — install from [nerdfonts.com](https://www.nerdfonts.com/).

## Alternatives
- [starship](starship.md)
- [oh-my-zsh](oh-my-zsh.md)
