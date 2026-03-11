# doggo

> Human-friendly command-line DNS client — a modern alternative to dig.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://doggo.mrkaran.dev/)
- [GitHub Repository](https://github.com/mr-karan/doggo) ⭐ 4.2k

## Install

### macOS
```bash
brew install doggo
```

### Linux
```bash
# Shell script
curl -fsSL https://raw.githubusercontent.com/mr-karan/doggo/main/install.sh | sh

# Go install
go install github.com/mr-karan/doggo/cmd/doggo@latest

# Download binary from releases
# https://github.com/mr-karan/doggo/releases
```

### Windows
```bash
# Scoop
scoop install doggo

# winget
winget install mr-karan.doggo

# Go install
go install github.com/mr-karan/doggo/cmd/doggo@latest
```

## Overview

doggo presents DNS query results in a clean, colorized table instead of dig's dense output. It supports all common record types and modern DNS protocols including DNS-over-HTTPS (DoH), DNS-over-TLS (DoT), and DNS-over-QUIC (DoQ).

```bash
# Basic lookup
doggo example.com

# Query a specific record type
doggo MX example.com
doggo AAAA example.com
doggo TXT example.com

# Use a specific nameserver
doggo example.com @8.8.8.8

# Use DNS-over-HTTPS
doggo example.com @https://cloudflare-dns.com/dns-query

# Use DNS-over-TLS
doggo example.com @tls://1.1.1.1

# JSON output
doggo --json example.com | jq
```
