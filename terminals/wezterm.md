# WezTerm

> GPU-accelerated terminal emulator and multiplexer with Lua-based configuration.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://wezterm.org)
- [GitHub Repository](https://github.com/wezterm/wezterm) ⭐ 24.8k
- [Documentation](https://wezterm.org/config/files.html)

## Install

### macOS

```bash
brew install --cask wezterm
```

### Linux

**Debian/Ubuntu (apt):**

```bash
curl -fsSL https://apt.fury.io/wez/gpg.key \
  | sudo gpg --yes --dearmor -o /usr/share/keyrings/wezterm-fury.gpg
echo 'deb [signed-by=/usr/share/keyrings/wezterm-fury.gpg] https://apt.fury.io/wez/ * *' \
  | sudo tee /etc/apt/sources.list.d/wezterm.list
sudo chmod 644 /usr/share/keyrings/wezterm-fury.gpg
sudo apt update && sudo apt install wezterm
```

**Flatpak:**

```bash
flatpak install flathub org.wezfurlong.wezterm
```

### Windows

```powershell
winget install wez.wezterm
```

Or via Scoop:

```powershell
scoop bucket add extras
scoop install wezterm
```

## Alternatives
- [kitty.md](kitty.md)
- [ghostty.md](ghostty.md)
