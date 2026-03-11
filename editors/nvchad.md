# NvChad

> Blazing fast Neovim configuration framework with a beautiful UI and solid defaults, built with Lua.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://nvchad.com/)
- [GitHub Repository](https://github.com/NvChad/NvChad) ⭐ 28k
- [Installation Guide](https://nvchad.com/docs/quickstart/install/)

## Install

Requires [Neovim](neovim.md) 0.10 or newer.

### macOS / Linux

Backup your existing Neovim config first:
```bash
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```

Clone the NvChad starter:
```bash
git clone https://github.com/NvChad/starter ~/.config/nvim && nvim
```

After plugins are installed, run `:MasonInstallAll` inside Neovim. Then delete the `.git` folder:
```bash
rm -rf ~/.config/nvim/.git
```

### Windows (PowerShell)

Backup your existing Neovim config first:
```powershell
Remove-Item -Force $ENV:USERPROFILE\AppData\Local\nvim-data
```

Clone the NvChad starter:
```powershell
git clone https://github.com/NvChad/starter $ENV:USERPROFILE\AppData\Local\nvim
nvim
```

After plugins are installed, run `:MasonInstallAll` inside Neovim.

## Alternatives
- [AstroNvim](astronvim.md)
- [LazyVim](lazyvim.md)
