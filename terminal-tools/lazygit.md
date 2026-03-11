# Lazygit

> Simple terminal UI for Git commands.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/jesseduffield/lazygit)

## Install

### macOS

```bash
brew install lazygit
```

### Linux

**Arch Linux:**

```bash
sudo pacman -S lazygit
```

**Ubuntu/Debian (via binary release):**

```bash
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": *"v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/v${LAZYGIT_VERSION}/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit -D -t /usr/local/bin/
```

**Fedora/RHEL:**

```bash
sudo dnf copr enable dejan/lazygit
sudo dnf install lazygit
```

### Windows

```bash
winget install JesseDuffield.lazygit
```

Or via Scoop:

```bash
scoop bucket add extras
scoop install lazygit
```

## Alternatives
- [git.md](git.md) — the underlying version control system
