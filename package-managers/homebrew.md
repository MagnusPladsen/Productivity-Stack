# Homebrew

> The missing package manager for macOS and Linux.

**Platforms:** macOS, Linux

## Links
- [Official Website](https://brew.sh/)
- [Documentation](https://docs.brew.sh/)
- [GitHub Repository](https://github.com/Homebrew/brew) ⭐ 47.0k

## Install

### macOS

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Linux

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

After installing on Linux, follow the instructions to add Homebrew to your PATH:

```bash
echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> ~/.bashrc
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```

## Notes

- On Apple Silicon Macs, Homebrew installs to `/opt/homebrew`
- On Intel Macs, Homebrew installs to `/usr/local`
- On Linux, Homebrew installs to `/home/linuxbrew/.linuxbrew`
- Homebrew on Linux was formerly known as Linuxbrew
