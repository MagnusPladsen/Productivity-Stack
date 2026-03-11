# yazi

> Blazing-fast terminal file manager written in Rust, with image previews and async I/O.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://yazi-rs.github.io/)
- [GitHub Repository](https://github.com/sxyazi/yazi)
- [Installation Docs](https://yazi-rs.github.io/docs/installation/)

## Install

### macOS

```bash
brew install yazi
```

With optional dependencies for full feature support:

```bash
brew install yazi ffmpegthumbnailer sevenzip jq poppler fd ripgrep fzf zoxide imagemagick font-symbols-only-nerd-font
```

### Linux

**Arch Linux:**

```bash
sudo pacman -S yazi
```

**Via Snap (Debian/Ubuntu):**

```bash
sudo snap install yazi
```

Or download a prebuilt binary from the [GitHub releases page](https://github.com/sxyazi/yazi/releases).

### Windows

```bash
winget install sxyazi.yazi
```

Or via Scoop:

```bash
scoop install yazi
```

## Alternatives
- [fd.md](fd.md) — fast file finder that pairs well with yazi for scripted file operations
- [fzf.md](fzf.md) — fuzzy finder for quick file selection without a full file manager
