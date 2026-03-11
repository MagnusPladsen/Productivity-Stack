# VSCodium

> Free, open-source build of VS Code without Microsoft telemetry, tracking, or proprietary licensing.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://vscodium.com)
- [GitHub Repository](https://github.com/VSCodium/vscodium) ⭐ 30.4k

## Install

### macOS

```bash
brew install --cask vscodium
```

### Linux

**Debian/Ubuntu (apt):**

```bash
wget -qO - https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/raw/master/pub.gpg \
  | gpg --dearmor \
  | sudo dd of=/usr/share/keyrings/vscodium-archive-keyring.gpg

echo 'deb [arch=amd64,arm64 signed-by=/usr/share/keyrings/vscodium-archive-keyring.gpg] https://download.vscodium.com/debs vscodium main' \
  | sudo tee /etc/apt/sources.list.d/vscodium.list > /dev/null

sudo apt update && sudo apt install codium
```

**Snap:**

```bash
sudo snap install codium --classic
```

### Windows

```powershell
winget install -e --id VSCodium.VSCodium
```

Or via Chocolatey:

```powershell
choco install vscodium
```

## Alternatives
- [vscode.md](vscode.md)
- [zed.md](zed.md)
