# Flameshot

> Powerful, open-source screenshot tool with built-in annotation, blur, arrows, text, and copy-to-clipboard — works at capture time without a separate editor.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://flameshot.org)
- [GitHub Repository](https://github.com/flameshot-org/flameshot)
- [Documentation](https://flameshot.org/docs/installation/)

## Install

### macOS
```bash
brew install --cask flameshot
```

> On first launch, grant Screen Recording permission in System Settings > Privacy & Security > Screen Recording. On macOS 15+, if the app is blocked, run: `sudo xattr -rd com.apple.quarantine /Applications/flameshot.app`

### Linux

**Debian/Ubuntu:**
```bash
sudo apt install flameshot
```

**Arch Linux:**
```bash
sudo pacman -S flameshot
```

**Flatpak:**
```bash
flatpak install flathub org.flameshot.Flameshot
```

### Windows

Download the `.msi` installer from the [GitHub Releases page](https://github.com/flameshot-org/flameshot/releases) and run it.

## Alternatives

For macOS-specific screenshot tools with OCR and pixel tools, see [Shottr](../productivity-tools/shottr.md).
