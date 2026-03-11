# git-absorb

> Automatically absorb staged changes into the most appropriate commit in your branch.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/tummychow/git-absorb)

## Install

### macOS
```bash
brew install git-absorb
```

### Linux
```bash
# Cargo
cargo install git-absorb

# Arch Linux
sudo pacman -S git-absorb
```

### Windows
```bash
# Cargo
cargo install git-absorb

# Or download binary from releases
# https://github.com/tummychow/git-absorb/releases
```

## Overview

git-absorb is the automated version of `git commit --fixup`. It analyzes your staged changes, figures out which existing commits in your branch they logically belong to, and creates `fixup!` commits accordingly. You then run `git rebase --autosquash` to clean everything up.

This avoids the manual cycle of: find the right commit hash, `git commit --fixup <hash>`, rebase.

```bash
# Stage some changes
git add -p

# Let git-absorb figure out where they belong
git absorb

# Then squash the fixup commits in
git rebase --autosquash origin/main

# Or do both in one step
git absorb --and-rebase
```

git-absorb only considers commits that are safe to modify (i.e., not yet pushed to a shared branch, or explicitly allowed). It will not create fixup commits for changes it can't confidently attribute to a single commit.

## Alternatives
- [lazygit](lazygit.md)
- [gitui](gitui.md)
