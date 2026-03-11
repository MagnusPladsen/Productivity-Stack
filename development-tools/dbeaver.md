# DBeaver

> Universal database management tool with SQL editor, ER diagrams, and data export.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://dbeaver.io/)
- [GitHub Repository](https://github.com/dbeaver/dbeaver)
- [Documentation](https://dbeaver.com/docs/dbeaver/)

## Install

### macOS

```bash
brew install --cask dbeaver-community
```

### Linux

**Snap:**

```bash
sudo snap install dbeaver-ce --classic
```

**APT (Debian/Ubuntu via official repo):**

```bash
wget -O - https://dbeaver.io/debs/dbeaver.gpg.key | sudo apt-key add -
echo "deb https://dbeaver.io/debs/dbeaver-ce /" | sudo tee /etc/apt/sources.list.d/dbeaver.list
sudo apt-get update && sudo apt-get install dbeaver-ce
```

### Windows

```bash
winget install dbeaver.dbeaver
```
