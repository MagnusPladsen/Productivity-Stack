# thefuck

> Magnificent app that auto-corrects your previous mistyped console command.

**Platforms:** macOS, Linux

## Links
- [GitHub Repository](https://github.com/nvbn/thefuck)

## Install

### macOS

```bash
brew install thefuck
```

Then add the alias to your shell config (`.zshrc` or `.bashrc`):

```bash
eval $(thefuck --alias)
```

### Linux

**Debian/Ubuntu:**

```bash
sudo apt install python3-dev python3-pip python3-setuptools
pip3 install thefuck --user
```

**Arch Linux:**

```bash
sudo pacman -S thefuck
```

**Other distributions (via pip):**

```bash
pip install thefuck
```

Then add the alias to your shell config:

```bash
eval $(thefuck --alias)
```

## Alternatives
- [tldr.md](tldr.md) — for looking up the correct command syntax before making a mistake
- [zoxide.md](zoxide.md) — smarter directory navigation that reduces common `cd` errors
