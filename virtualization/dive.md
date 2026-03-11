# dive

> Interactive TUI for exploring Docker image layers and finding ways to shrink image size.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/wagoodman/dive) ⭐ 53.5k

## Install

### macOS
```bash
brew install dive
```

### Linux
```bash
# Download and install latest .deb (Ubuntu/Debian)
DIVE_VERSION=$(curl -sL "https://api.github.com/repos/wagoodman/dive/releases/latest" \
  | grep '"tag_name":' | sed -E 's/.*"v([^"]+)".*/\1/')
curl -fOL "https://github.com/wagoodman/dive/releases/download/v${DIVE_VERSION}/dive_${DIVE_VERSION}_linux_amd64.deb"
sudo apt install ./dive_${DIVE_VERSION}_linux_amd64.deb
```

### Windows
```bash
# Via Go
go install github.com/wagoodman/dive@latest
```

## Usage
```bash
dive nginx:latest          # Explore a local or remote image
```
