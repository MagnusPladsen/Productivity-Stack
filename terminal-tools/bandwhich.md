# bandwhich

> Real-time terminal UI showing network bandwidth usage broken down by process and connection.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/imsnif/bandwhich)

## Install

### macOS
```bash
brew install bandwhich
```

### Linux
```bash
cargo install bandwhich

# Or build from source (requires libpcap-dev)
sudo apt install build-essential libpcap-dev
cargo build --release
```

### Windows
```bash
cargo install bandwhich
```

## Overview

bandwhich sniffs network packets and shows a live TUI with three panes: per-process bandwidth usage, per-connection details, and per-remote-IP/hostname totals. It resolves hostnames in real time and updates continuously.

Because it requires raw packet capture, it must be run with elevated privileges:

```bash
sudo bandwhich
```

On Linux you can grant capabilities to the binary to avoid sudo:
```bash
sudo setcap cap_sys_ptrace,cap_dac_read_search,cap_net_raw,cap_net_admin+ep $(which bandwhich)
bandwhich
```

## Alternatives
- [htop](htop.md)
- [bottom](bottom.md)
