# Netdata

> Real-time infrastructure monitoring with 1-second resolution and zero configuration.

**Platforms:** macOS, Linux

> **Agent:** 100% free and open source, self-hosted.
> **Cloud:** Free community tier available; paid plans add longer retention, advanced alerts, and team features.

## Links
- [Official Website](https://netdata.cloud)
- [GitHub Repository](https://github.com/netdata/netdata)

## Install

### macOS
```bash
brew install netdata
sudo brew services start netdata
```

### Linux
```bash
# One-line kickstart script (all major distros)
curl https://get.netdata.cloud/kickstart.sh > /tmp/netdata-kickstart.sh && sh /tmp/netdata-kickstart.sh
```

Once running, open [http://localhost:19999](http://localhost:19999) in your browser.

## Alternatives
- [Grafana](grafana.md) — dashboard and visualization platform (pairs well with Netdata as a data source)
