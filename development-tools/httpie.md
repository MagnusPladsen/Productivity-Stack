# HTTPie

> Human-friendly HTTP client for the CLI and desktop — with JSON support, syntax highlighting, and sessions.

**Platforms:** macOS, Linux, Windows

**Pricing:** CLI is 100% free and open source. Desktop app has a free tier (limited to 5 collections and basic features); paid plans unlock unlimited collections and team features.

## Links
- [Official Website](https://httpie.io)
- [GitHub Repository](https://github.com/httpie/cli) ⭐ 37.7k
- [Documentation](https://httpie.io/docs/cli)

## Install

### macOS

```bash
brew install httpie
```

### Linux

**Debian/Ubuntu:**

```bash
curl -SsL https://packages.httpie.io/deb/KEY.gpg | sudo gpg --dearmor -o /usr/share/keyrings/httpie.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/httpie.gpg] https://packages.httpie.io/deb ./" \
  | sudo tee /etc/apt/sources.list.d/httpie.list > /dev/null
sudo apt update && sudo apt install httpie
```

**pip (any distro):**

```bash
python -m pip install --upgrade httpie
```

### Windows

**pip:**

```bash
python -m pip install --upgrade pip wheel
python -m pip install httpie
```

**Chocolatey:**

```bash
choco install httpie
```

## Alternatives
- [bruno.md](bruno.md)
- [postman.md](postman.md)
