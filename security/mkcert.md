# mkcert

> Zero-config tool to create locally trusted HTTPS certificates for development.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/FiloSottile/mkcert)

## Install

### macOS
```bash
brew install mkcert
brew install nss  # required if using Firefox
```

### Linux
```bash
# Install nss-tools first (required for Firefox/Chrome)
# Ubuntu/Debian:
sudo apt install libnss3-tools

# Arch:
sudo pacman -S nss

# Then install mkcert via Homebrew on Linux:
brew install mkcert

# Or on Arch directly:
sudo pacman -S mkcert
```

### Windows
```bash
winget install -e --id FiloSottile.mkcert
```

## Usage
```bash
mkcert -install                        # Install local CA
mkcert localhost 127.0.0.1 ::1        # Generate cert for localhost
```
