# croc

> Easily and securely send files and folders between computers.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://schollz.com/software/croc/)
- [GitHub Repository](https://github.com/schollz/croc) ⭐ 34.3k

## Install

### macOS
```bash
brew install croc
```

### Linux
```bash
curl https://getcroc.schollz.com | sudo bash
```

Or via package manager on supported distros:
```bash
# Arch Linux
sudo pacman -S croc

# Fedora
sudo dnf install croc
```

### Windows
```bash
winget install schollz.croc
```

## Overview

croc uses a relay server to connect any two computers without requiring port forwarding. It encrypts all transfers end-to-end using PAKE (password-authenticated key exchange), and supports resuming interrupted transfers. Both sender and receiver need croc installed — the sender generates a short code phrase that the receiver enters to accept the transfer.

```bash
# Send a file
croc send file.txt

# Receive (on another machine)
croc <code-phrase>

# Send a folder
croc send my-folder/
```

## Free Tier

100% free and open source. Uses a public relay server by default. You can self-host your own relay with `croc relay`.

## Alternatives
- [curl](curl.md)
