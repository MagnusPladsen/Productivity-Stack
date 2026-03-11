# delta

> Syntax-highlighting pager for git diffs, blame, grep, and show output.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://dandavison.github.io/delta/)
- [GitHub Repository](https://github.com/dandavison/delta)

## Install

### macOS
```bash
brew install git-delta
```

### Linux
```bash
# Debian/Ubuntu — download .deb from releases page:
# https://github.com/dandavison/delta/releases
# Then install with:
sudo dpkg -i git-delta_*.deb

# Arch Linux
sudo pacman -S git-delta

# Fedora
sudo dnf install git-delta
```

### Windows
```bash
winget install dandavison.delta
```

## Setup

After installing, configure git to use delta as the pager:

```bash
git config --global core.pager delta
git config --global interactive.diffFilter "delta --color-only"
git config --global delta.navigate true
git config --global merge.conflictstyle diff3
git config --global diff.colorMoved default
```

## Alternatives
- [bat](bat.md)
