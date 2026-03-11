# Brave

> Chromium-based browser with built-in ad and tracker blocking, fingerprinting protection, and an optional privacy-preserving ad rewards system.

**Platforms:** macOS, Linux, Windows

**Pricing:** 100% free. Optional Brave VPN is paid ($9.99/month).

## Links
- [Official Website](https://brave.com)
- [GitHub Repository](https://github.com/brave/brave-browser) ⭐ 21.9k

## Install

### macOS
```bash
brew install --cask brave-browser
```

### Linux

**Debian/Ubuntu:**
```bash
sudo curl -Lo /usr/share/keyrings/brave-browser-archive-keyring.gpg \
  https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] \
  https://brave-browser-apt-release.s3.brave.com/ stable main" \
  | sudo tee /etc/apt/sources.list.d/brave-browser-release.list

sudo apt update && sudo apt install -y brave-browser
```

### Windows
```bash
winget install -e --id Brave.Brave
```

## Alternatives
- [Firefox](firefox.md)
- [Zen Browser](zen-browser.md)
