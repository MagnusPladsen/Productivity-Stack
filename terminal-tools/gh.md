# gh

> GitHub's official CLI — manage pull requests, issues, and repos from the terminal.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://cli.github.com/)
- [GitHub Repository](https://github.com/cli/cli) ⭐ 43.1k
- [Linux Install Docs](https://github.com/cli/cli/blob/trunk/docs/install_linux.md)

## Install

### macOS

```bash
brew install gh
```

### Linux

**Debian/Ubuntu (official package):**

```bash
(type -p wget >/dev/null || (sudo apt update && sudo apt install wget -y)) \
  && sudo mkdir -p -m 755 /etc/apt/keyrings \
  && wget -qO- https://cli.github.com/packages/githubcli-archive-keyring.gpg \
     | sudo tee /etc/apt/keyrings/githubcli-archive-keyring.gpg > /dev/null \
  && sudo chmod go+r /etc/apt/keyrings/githubcli-archive-keyring.gpg \
  && echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" \
     | sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null \
  && sudo apt update \
  && sudo apt install gh -y
```

**Fedora:**

```bash
sudo dnf install gh
```

**Arch Linux:**

```bash
sudo pacman -S github-cli
```

### Windows

```bash
winget install GitHub.cli
```

Or via Scoop:

```bash
scoop install gh
```

Or via Chocolatey:

```bash
choco install gh
```

## Alternatives
- [lazygit.md](lazygit.md) — TUI for local git operations, complements gh for GitHub-specific workflows
- [git.md](git.md) — the underlying VCS gh wraps around
