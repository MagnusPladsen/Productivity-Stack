# mise

> Polyglot runtime version manager — a single tool to manage Node.js, Python, Ruby, Go, Rust, Java, and hundreds more, replacing nvm, pyenv, rbenv, and asdf.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://mise.jdx.dev/)
- [GitHub Repository](https://github.com/jdx/mise) ⭐ 25.5k

## Install

### macOS
```bash
brew install mise
```

### Linux
```bash
# apt (Debian/Ubuntu)
sudo apt install -y mise

# Install script
curl https://mise.run | sh
```

### Windows
```bash
winget install jdx.mise
```

## Setup

Add the shell activation line after installing:

```bash
# Bash (~/.bashrc)
eval "$(mise activate bash)"

# Zsh (~/.zshrc)
eval "$(mise activate zsh)"

# Fish (~/.config/fish/config.fish)
mise activate fish | source
```

## Usage

```bash
# Install a runtime
mise use node@22
mise use python@3.12

# List installed versions
mise list

# Set a global default
mise use --global node@lts
```
