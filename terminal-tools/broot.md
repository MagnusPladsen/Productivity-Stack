# broot

> Interactive directory tree navigator — browse large trees, fuzzy-search, preview files, and run commands without losing context.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://dystroy.org/broot/)
- [GitHub Repository](https://github.com/Canop/broot)

## Install

### macOS
```bash
brew install broot
```

### Linux
```bash
# Cargo (requires Rust — recommended for latest version)
cargo install broot

# Arch Linux (AUR)
yay -S broot
```

### Windows
```bash
# Cargo (requires Rust)
cargo install broot

# Scoop
scoop install broot
```

## Setup

After installing, run the shell function installer so `br` can change your working directory:

```bash
broot --install
```

Then use `br` instead of `broot` to get `cd`-on-enter behavior.

## Alternatives
- [yazi](yazi.md)
- [eza](eza.md)
