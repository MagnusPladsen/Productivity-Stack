# bottom

> Graphical cross-platform process and system monitor with customizable widgets for CPU, memory, disk, network, and processes. Invoked as `btm`.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://clementtang.github.io/bottom/)
- [GitHub Repository](https://github.com/ClementTsang/bottom)

## Install

### macOS
```bash
brew install bottom
```

### Linux
```bash
# Cargo (requires Rust)
cargo install bottom --locked

# Arch Linux
sudo pacman -S bottom
```

### Windows
```bash
winget install Clement.bottom
```

## Usage

```bash
# Launch
btm

# Show all processes (default view focuses on resource-heavy ones)
btm --basic
```

## Alternatives
- [htop](htop.md)
