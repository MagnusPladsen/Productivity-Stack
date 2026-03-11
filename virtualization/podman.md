# Podman

> Rootless, daemonless container engine — a drop-in Docker alternative.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://podman.io)
- [GitHub Repository](https://github.com/containers/podman) ⭐ 31.0k

## Install

### macOS
```bash
brew install podman
podman machine init
podman machine start
```

### Linux
```bash
# Ubuntu/Debian
sudo apt update
sudo apt install podman

# Fedora/RHEL
sudo dnf install podman
```

### Windows
```bash
winget install -e --id RedHat.Podman
```

After installation on Windows, initialize a machine:
```bash
podman machine init
podman machine start
```

## Alternatives
- [Docker](../development-tools/docker.md) — the original container runtime
