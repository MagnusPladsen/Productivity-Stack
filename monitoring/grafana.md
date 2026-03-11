# Grafana

> Open-source dashboard and visualization platform for metrics, logs, and traces.

**Platforms:** macOS, Linux, Windows

> **Self-hosted:** 100% free (OSS edition).
> **Grafana Cloud:** Free tier includes 10k metrics, 50 GB logs, 50 GB traces, 500 GB profiles, 3 active users.

## Links
- [Official Website](https://grafana.com)
- [GitHub Repository](https://github.com/grafana/grafana)

## Install

### macOS
```bash
brew install grafana
brew services start grafana
```

### Linux
```bash
# Ubuntu/Debian — add official APT repository
sudo mkdir -p /etc/apt/keyrings
sudo wget -O /etc/apt/keyrings/grafana.asc https://apt.grafana.com/gpg-full.key
echo "deb [signed-by=/etc/apt/keyrings/grafana.asc] https://apt.grafana.com stable main" \
  | sudo tee /etc/apt/sources.list.d/grafana.list
sudo apt-get update
sudo apt-get install grafana
sudo systemctl enable --now grafana-server
```

### Windows
Download the installer from [grafana.com/grafana/download](https://grafana.com/grafana/download?platform=windows).

Once running, open [http://localhost:3000](http://localhost:3000) in your browser (default credentials: `admin` / `admin`).

## Alternatives
- [Netdata](netdata.md) — zero-config real-time monitoring agent
