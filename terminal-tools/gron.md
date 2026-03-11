# gron

> Make JSON greppable by flattening it into discrete path assignments.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://github.com/tomnomnom/gron)
- [GitHub Repository](https://github.com/tomnomnom/gron) ⭐ 14.4k

## Install

### macOS
```bash
brew install gron
```

### Linux
```bash
# Download binary from releases
# https://github.com/tomnomnom/gron/releases

# Go install
go install github.com/tomnomnom/gron@latest
```

### Windows
```bash
# Go install
go install github.com/tomnomnom/gron@latest

# Or download binary from releases
# https://github.com/tomnomnom/gron/releases
```

## Overview

gron transforms nested JSON into flat, grep-friendly path assignments. Each value appears on its own line with its full dot-notation path, making it trivial to search through deeply nested JSON with standard Unix tools. You can pipe the output back through `gron --ungron` (or `gronx`) to reconstitute JSON from filtered results.

```bash
# Flatten JSON for grepping
curl https://api.github.com/repos/tomnomnom/gron | gron

# Output looks like:
# json = {};
# json.description = "Make JSON greppable!";
# json.stargazers_count = 12345;

# Grep for a value and ungron back to JSON
curl https://api.github.com/repos/tomnomnom/gron | gron | grep "stargazers" | gron --ungron
```

## Alternatives
- [jq](jq.md)
- [fx](fx.md)
