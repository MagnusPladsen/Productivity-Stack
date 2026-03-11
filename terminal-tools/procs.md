# procs

> A modern, colorful replacement for ps written in Rust.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/dalance/procs) ⭐ 6.0k

## Install

### macOS
```bash
brew install procs
```

### Linux
```bash
# Cargo
cargo install procs

# Arch Linux
sudo pacman -S procs

# Alpine Linux
apk add procs

# Snap
sudo snap install procs
```

### Windows
```bash
# Scoop
scoop install procs

# Cargo
cargo install procs
```

## Overview

procs presents process information in color-coded, human-readable columns with smart defaults. It shows TCP/UDP port bindings, Docker container names, read/write throughput, and memory details that `ps` doesn't expose easily. It also supports a tree view, watch mode, and fuzzy keyword search across all columns.

```bash
# List all processes
procs

# Search for a process by name or any column value
procs nginx

# Tree view showing parent/child relationships
procs --tree

# Watch mode (like top)
procs --watch

# Show only specific columns
procs --sortd cpu

# Insert config for shell completion and default settings
procs --gen-config > ~/.config/procs/config.toml
```

## Alternatives
- [htop](htop.md)
- [bottom](bottom.md)
