# dust

> Visual disk usage tool that shows a tree of directories sorted by size — a more intuitive replacement for `du`.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://github.com/bootandy/dust)
- [GitHub Repository](https://github.com/bootandy/dust)

## Install

### macOS
```bash
brew install dust
```

### Linux
```bash
# Cargo (requires Rust)
cargo install du-dust

# Arch Linux
sudo pacman -S dust

# Download .deb from releases and install manually:
# https://github.com/bootandy/dust/releases
sudo dpkg -i dust_*.deb
```

### Windows
```bash
winget install bootandy.dust
```

## Usage

```bash
# Show disk usage of current directory
dust

# Limit depth
dust -d 3

# Show usage of a specific directory
dust /var/log
```

## Alternatives
- [ncdu](ncdu.md)
