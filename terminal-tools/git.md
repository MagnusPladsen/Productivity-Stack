# Git

> Distributed version control system for tracking changes in source code.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://git-scm.com/)
- [Installation Docs](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Install

### macOS

Git is bundled with Xcode Command Line Tools. Run the following to install if not already present:

```bash
xcode-select --install
```

Or install the latest version via Homebrew:

```bash
brew install git
```

### Linux

**Debian/Ubuntu:**

```bash
sudo apt install git
```

**Fedora:**

```bash
sudo dnf install git
```

**Arch Linux:**

```bash
sudo pacman -S git
```

**RHEL/CentOS:**

```bash
sudo yum install git
```

### Windows

```bash
winget install --id Git.Git -e --source winget
```

Or download the installer from [git-scm.com/download/win](https://git-scm.com/download/win).

## Alternatives
- [lazygit.md](lazygit.md) — terminal UI built on top of Git for a more visual workflow
