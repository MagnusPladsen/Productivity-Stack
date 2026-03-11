# fzf

> A general-purpose command-line fuzzy finder for files, history, processes, and more.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/junegunn/fzf)
- [Official Docs](https://junegunn.github.io/fzf/)
- [Installation Guide](https://junegunn.github.io/fzf/installation/)

## Install

### macOS

```bash
brew install fzf
```

### Linux

**Debian/Ubuntu:**

```bash
sudo apt install fzf
```

**Fedora:**

```bash
sudo dnf install fzf
```

**Arch Linux:**

```bash
sudo pacman -S fzf
```

Via Git (all Linux distros, also installs shell integration):

```bash
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
```

### Windows

```bash
winget install junegunn.fzf
```

Or via Scoop:

```bash
scoop install fzf
```

Or via Chocolatey:

```bash
choco install fzf
```

## Alternatives
- [fd.md](fd.md) — fast find alternative that pairs naturally with fzf for file selection
- [zoxide.md](zoxide.md) — smarter cd that complements fzf for directory navigation
