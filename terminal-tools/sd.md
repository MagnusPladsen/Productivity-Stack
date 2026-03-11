# sd

> Intuitive find-and-replace CLI — a simpler, faster alternative to sed.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/chmln/sd) ⭐ 7.0k

## Install

### macOS
```bash
brew install sd
```

### Linux
```bash
cargo install sd

# Arch Linux
sudo pacman -S sd
```

### Windows
```bash
cargo install sd
```

## Overview

sd uses the same regex syntax as JavaScript and Python, making it far more approachable than sed's POSIX regex. It also handles multi-line replacements cleanly and edits files in-place by default.

```bash
# Replace in a string
echo 'hello world' | sd 'world' 'there'

# Replace in a file (in-place)
sd 'foo' 'bar' file.txt

# Replace across multiple files
sd 'oldFunction' 'newFunction' src/**/*.ts

# Use capture groups
echo '2024-01-15' | sd '(\d{4})-(\d{2})-(\d{2})' '$3/$2/$1'
# Output: 15/01/2024

# Fixed-string mode (no regex)
sd -F 'foo.bar' 'baz' file.txt
```

Compared to sed:
```bash
# sed (POSIX regex, hard to remember)
sed -i 's/old/new/g' file.txt

# sd (intuitive, same result)
sd 'old' 'new' file.txt
```
