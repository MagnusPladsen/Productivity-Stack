# chezmoi

> Dotfile manager with templating, secrets integration, and cross-machine sync — manage dotfiles across multiple machines from a single source of truth.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://www.chezmoi.io/)
- [GitHub Repository](https://github.com/twpayne/chezmoi)

## Install

### macOS
```bash
brew install chezmoi
```

### Linux
```bash
# Universal install script (places binary in ~/.local/bin):
sh -c "$(curl -fsLS get.chezmoi.io)"

# Snap
sudo snap install chezmoi --classic
```

### Windows
```bash
winget install twpayne.chezmoi
```

## Quick Start

```bash
# Initialize with an existing dotfiles GitHub repo
chezmoi init --apply <github-username>

# Add a file to be managed
chezmoi add ~/.zshrc

# Apply changes
chezmoi apply
```
