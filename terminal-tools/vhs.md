# vhs

> Record terminal GIFs and videos from a script file.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://charm.sh/)
- [GitHub Repository](https://github.com/charmbracelet/vhs)

## Install

### macOS
```bash
brew install vhs
```

### Linux
```bash
# Charm apt repository
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://repo.charm.sh/apt/gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/charm.gpg
echo "deb [signed-by=/etc/apt/keyrings/charm.gpg] https://repo.charm.sh/apt/ * *" | sudo tee /etc/apt/sources.list.d/charm.list
sudo apt update && sudo apt install vhs ffmpeg

# Arch Linux
sudo pacman -S vhs

# Nix
nix-env -iA nixpkgs.vhs
```

### Windows
```bash
scoop install vhs
```

## Dependencies

vhs requires `ttyd` and `ffmpeg` to be installed and available on your PATH:

```bash
# macOS
brew install ttyd ffmpeg

# Ubuntu/Debian
sudo apt install ttyd ffmpeg
```

## Overview

vhs lets you write `.tape` scripts that describe terminal interactions — keystrokes, pauses, commands — and renders them into a GIF or MP4. This makes it easy to produce reproducible, pixel-perfect terminal demos for documentation and READMEs.

```tape
Output demo.gif

Set FontSize 14
Set Width 1200
Set Height 600

Type "echo 'Hello, world!'"
Enter
Sleep 1s
```

```bash
# Record from a tape file
vhs demo.tape
```

## Alternatives
- [asciinema](asciinema.md)
