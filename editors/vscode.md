# Visual Studio Code

> Lightweight but powerful source code editor with built-in support for debugging, Git, and a rich extension ecosystem.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://code.visualstudio.com/)
- [GitHub Repository](https://github.com/microsoft/vscode)
- [Documentation](https://code.visualstudio.com/docs)
- [Extension Marketplace](https://marketplace.visualstudio.com/vscode)

## Install

### macOS
```bash
brew install --cask visual-studio-code
```

### Linux
```bash
# Snap (recommended)
sudo snap install code --classic

# Debian / Ubuntu (apt)
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings/packages.microsoft.gpg
echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" | sudo tee /etc/apt/sources.list.d/vscode.list > /dev/null
sudo apt update && sudo apt install code
```

### Windows
```bash
winget install --id Microsoft.VisualStudioCode
```

## Alternatives
- [Zed](zed.md)
- [Neovim](neovim.md)
