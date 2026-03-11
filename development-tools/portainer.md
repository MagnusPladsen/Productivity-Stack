# Portainer

> Web UI for managing Docker and Kubernetes environments — containers, images, volumes, networks, and stacks.

**Platforms:** macOS, Linux, Windows (runs as a Docker container)

**Pricing:** Community Edition is 100% free and open source with no node limits. Business Edition has a free tier for up to 3 nodes (requires annual license renewal); additional nodes are paid.

## Links
- [Official Website](https://portainer.io)
- [GitHub Repository](https://github.com/portainer/portainer)
- [Documentation](https://docs.portainer.io)

## Install

Portainer CE runs as a Docker container and manages your local Docker socket.

### macOS / Linux

```bash
docker volume create portainer_data

docker run -d \
  -p 8000:8000 \
  -p 9443:9443 \
  --name portainer \
  --restart=always \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v portainer_data:/data \
  portainer/portainer-ce:sts
```

### Windows (Docker Desktop / WSL2)

```powershell
docker volume create portainer_data

docker run -d `
  -p 8000:8000 `
  -p 9443:9443 `
  --name portainer `
  --restart=always `
  -v /var/run/docker.sock:/var/run/docker.sock `
  -v portainer_data:/data `
  portainer/portainer-ce:sts
```

Once running, open [https://localhost:9443](https://localhost:9443) to access the UI.

## Alternatives
- [terminal-tools/lazydocker.md](../terminal-tools/lazydocker.md)
