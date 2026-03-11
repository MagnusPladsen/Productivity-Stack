# fd

> A simple, fast, and user-friendly alternative to find.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/sharkdp/fd)

## Install

### macOS

```bash
brew install fd
```

### Linux

**Debian/Ubuntu:**

```bash
sudo apt install fd-find
```

> Note: the binary is installed as `fdfind` on Debian/Ubuntu. Create an alias: `alias fd='fdfind'`

**Arch Linux:**

```bash
sudo pacman -S fd
```

**Fedora:**

```bash
sudo dnf install fd-find
```

**Void Linux:**

```bash
sudo xbps-install -S fd
```

### Windows

```bash
winget install sharkdp.fd
```

Or via Scoop:

```bash
scoop install fd
```

Or via Chocolatey:

```bash
choco install fd
```

## Alternatives
- [ripgrep.md](ripgrep.md) — fast grep alternative, pairs naturally with fd for searching file contents
- [fzf.md](fzf.md) — fuzzy finder that works great combined with fd for file selection
