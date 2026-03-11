# LazyVim

> Fast, modular Neovim configuration powered by lazy.nvim, designed to be easily extensible without starting from scratch.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://www.lazyvim.org/)
- [GitHub Repository](https://github.com/LazyVim/LazyVim)
- [Installation Guide](https://www.lazyvim.org/installation)

## Install

Requires [Neovim](neovim.md) 0.9 or newer.

### macOS / Linux

Backup your existing Neovim config first:
```bash
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```

Clone the LazyVim starter:
```bash
git clone https://github.com/LazyVim/starter ~/.config/nvim
rm -rf ~/.config/nvim/.git
nvim
```

### Windows (PowerShell)

Backup your existing Neovim config first:
```powershell
Move-Item $env:LOCALAPPDATA\nvim $env:LOCALAPPDATA\nvim.bak
```

Clone the LazyVim starter:
```powershell
git clone https://github.com/LazyVim/starter "$env:LOCALAPPDATA\nvim"
Remove-Item -Recurse -Force "$env:LOCALAPPDATA\nvim\.git"
nvim
```

## Alternatives
- [AstroNvim](astronvim.md)
- [NvChad](nvchad.md)
