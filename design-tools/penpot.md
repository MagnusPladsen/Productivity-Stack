# Penpot

> Open-source design and prototyping tool that works with open standards (SVG, CSS, HTML), built for designers and developers to collaborate.

**Platforms:** Web-based (macOS, Linux, Windows via browser); self-hostable

## Links
- [Official Website](https://penpot.app/)
- [GitHub Repository](https://github.com/penpot/penpot)
- [Self-Hosting Guide](https://help.penpot.app/technical-guide/getting-started/)

## Install

### Self-Hosted (Docker)
```bash
wget https://raw.githubusercontent.com/penpot/penpot/main/docker/images/docker-compose.yaml
docker compose -p penpot -f docker-compose.yaml up -d
```

> Penpot is primarily accessed via browser. The self-hosted option requires Docker and Docker Compose. A managed cloud version is available at [penpot.app](https://penpot.app/) with no installation required.

## Alternatives
- [draw-io](draw-io.md)
- [modulz](modulz.md)
