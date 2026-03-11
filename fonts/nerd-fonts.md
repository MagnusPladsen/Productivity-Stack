# Nerd Fonts

> 67+ patched developer fonts with 10,000+ icons from Font Awesome, Material Design, Devicons, and more.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://nerdfonts.com)
- [GitHub Repository](https://github.com/ryanoasis/nerd-fonts) ⭐ 62.0k

## Install

### macOS
```bash
# Search available fonts
brew search nerd-font

# Install a specific font (examples)
brew install --cask font-fira-code-nerd-font
brew install --cask font-jetbrains-mono-nerd-font
brew install --cask font-hack-nerd-font
```

### Linux
```bash
# Clone the repo and use the install script for a specific font
git clone --filter=blob:none --sparse https://github.com/ryanoasis/nerd-fonts.git
cd nerd-fonts
git sparse-checkout add patched-fonts/FiraCode
./install.sh FiraCode

# Or download a single font file directly
mkdir -p ~/.local/share/fonts
curl -fLo ~/.local/share/fonts/"FiraCode Nerd Font Complete.ttf" \
  https://github.com/ryanoasis/nerd-fonts/raw/HEAD/patched-fonts/FiraCode/Regular/FiraCodeNerdFont-Regular.ttf
fc-cache -fv
```

### Windows
```powershell
# Via PowerShell with NerdFonts module
Install-PSResource -Name NerdFonts
Import-Module -Name NerdFonts
Install-NerdFont -Name FiraCode
```

## Popular fonts
| Font | Notes |
|------|-------|
| FiraCode | Ligatures, great for coding |
| JetBrainsMono | Clean, designed for IDEs |
| Hack | Legible, minimal |
| CascadiaCode | Microsoft's coding font with ligatures |
