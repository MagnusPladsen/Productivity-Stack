# Signal

> End-to-end encrypted messaging and calls. No ads, no trackers, open source.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://signal.org)
- [GitHub Repository](https://github.com/signalapp/Signal-Desktop) ⭐ 16.1k

## Install

### macOS
```bash
brew install --cask signal
```

### Linux
```bash
# Official APT repository (Ubuntu/Debian)
wget -O- https://updates.signal.org/desktop/apt/keys.asc \
  | gpg --dearmor \
  | sudo tee /usr/share/keyrings/signal-desktop-keyring.gpg > /dev/null
wget -O signal-desktop.sources https://updates.signal.org/static/desktop/apt/signal-desktop.sources
sudo mv signal-desktop.sources /etc/apt/sources.list.d/
sudo apt update && sudo apt install signal-desktop
```

### Windows
```bash
winget install -e --id OpenWhisperSystems.Signal
```
