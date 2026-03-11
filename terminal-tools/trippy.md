# trippy

> Network diagnostic TUI that combines traceroute and ping into a single interactive view.

**Platforms:** macOS, Linux, Windows, BSD

## Links
- [Official Website](https://trippy.cli.rs/)
- [GitHub Repository](https://github.com/fujiapple852/trippy)

## Install

### macOS
```bash
brew install trippy
```

### Linux
```bash
# Ubuntu/Debian (PPA)
sudo add-apt-repository ppa:fujiapple/trippy
sudo apt update && sudo apt install trippy

# Cargo
cargo install trippy --locked

# Arch Linux
sudo pacman -S trippy

# Snap
sudo snap install trippy
```

### Windows
```bash
winget install -e --id FujiApple.Trippy
```

## Overview

trippy sends probes using ICMP, UDP, or TCP and renders a live TUI showing each network hop with round-trip time statistics, packet loss percentages, and jitter — all updating in real time. It's significantly more informative than running `traceroute` and `ping` separately.

Because it uses raw sockets, it requires elevated privileges:

```bash
# Basic trace to a host
sudo trip example.com

# Use TCP probes (useful when ICMP is blocked)
sudo trip --protocol tcp example.com

# Use UDP probes
sudo trip --protocol udp example.com

# Set max TTL
sudo trip --max-ttl 30 example.com
```

On Linux you can grant capabilities to avoid sudo:
```bash
sudo setcap cap_net_raw+p $(which trip)
```

## Alternatives
- [htop](htop.md)
