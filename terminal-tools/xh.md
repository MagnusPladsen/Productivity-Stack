# xh

> Friendly and fast HTTP client with HTTPie-compatible syntax.

**Platforms:** macOS, Linux, Windows

## Links
- [GitHub Repository](https://github.com/ducaale/xh) ⭐ 7.6k

## Install

### macOS
```bash
brew install xh
```

### Linux
```bash
# apt
sudo apt install xh

# Cargo
cargo install xh --locked

# Shell script
curl -sfL https://raw.githubusercontent.com/ducaale/xh/master/install.sh | sh
```

### Windows
```bash
# PowerShell
iwr -useb https://raw.githubusercontent.com/ducaale/xh/master/install.ps1 | iex

# Scoop
scoop install xh
```

## Overview

xh reimplements HTTPie's clean, expressive syntax with a focus on speed — it starts significantly faster than HTTPie and has no Python dependency. Requests are specified in a human-readable shorthand rather than raw curl flags.

```bash
# GET request
xh httpbin.org/get

# POST JSON
xh POST httpbin.org/post name=alice age:=30

# Add headers
xh GET api.example.com Authorization:"Bearer token"

# Download a file
xh --download example.com/file.zip

# Use as a curl-compatible alias (xhs for HTTPS)
xhs api.example.com/users

# Follow redirects and show verbose output
xh -v --follow httpbin.org/redirect/3
```

Data item types: `key=value` (string), `key:=value` (raw JSON), `key==value` (query param), `key@file` (file upload).

## Alternatives
- [curl](curl.md)
