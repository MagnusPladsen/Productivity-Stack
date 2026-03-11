# AstroNvim

> Aesthetic and feature-rich Neovim distribution that is extensible and easy to use with a great set of plugins.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://astronvim.com/)
- [GitHub Repository](https://github.com/AstroNvim/AstroNvim) ⭐ 14.2k
- [Documentation](https://docs.astronvim.com/)

## Install

Requires [Neovim](neovim.md) 0.10 or newer.

### macOS / Linux

Backup your existing Neovim config first:
```bash
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```

Clone the AstroNvim template:
```bash
git clone --depth 1 https://github.com/AstroNvim/template ~/.config/nvim
rm -rf ~/.config/nvim/.git
nvim
```

### Windows (PowerShell)

Backup your existing Neovim config first:
```powershell
Move-Item $env:LOCALAPPDATA\nvim $env:LOCALAPPDATA\nvim.bak
```

Clone the AstroNvim template:
```powershell
git clone --depth 1 https://github.com/AstroNvim/template $env:LOCALAPPDATA\nvim
Remove-Item $env:LOCALAPPDATA\nvim\.git -Recurse -Force
nvim
```

## Alternatives
- [LazyVim](lazyvim.md)
- [NvChad](nvchad.md)
