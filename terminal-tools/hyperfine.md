# hyperfine

> Statistical command-line benchmarking tool — runs commands multiple times, warms up caches, and reports mean, standard deviation, and outliers.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://github.com/sharkdp/hyperfine)
- [GitHub Repository](https://github.com/sharkdp/hyperfine)

## Install

### macOS
```bash
brew install hyperfine
```

### Linux
```bash
sudo apt install hyperfine
```

### Windows
```bash
winget install hyperfine
```

## Usage

```bash
# Basic benchmark
hyperfine 'sleep 0.3'

# Compare two commands
hyperfine 'find . -name "*.rs"' 'fd -e rs'

# Warmup runs before timing
hyperfine --warmup 3 'grep -r TODO .'
```
