# zoxide

> A smarter cd command that learns your most-visited directories.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/ajeetdsouza/zoxide)

## Install

### macOS

```bash
brew install zoxide
```

### Linux

**Debian/Ubuntu:**

```bash
sudo apt install zoxide
```

**Fedora:**

```bash
sudo dnf install zoxide
```

**Arch Linux:**

```bash
sudo pacman -S zoxide
```

### Windows

```bash
winget install ajeetdsouza.zoxide
```

Or via Scoop:

```bash
scoop install zoxide
```

## Post-install shell setup

After installing, add the init line to your shell config:

**Zsh** (`~/.zshrc`):

```bash
eval "$(zoxide init zsh)"
```

**Bash** (`~/.bashrc`):

```bash
eval "$(zoxide init bash)"
```

**Fish** (`~/.config/fish/config.fish`):

```bash
zoxide init fish | source
```

## Alternatives
- [fzf.md](fzf.md) — fuzzy finder that pairs well with zoxide for interactive directory selection
