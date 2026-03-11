# Hoppscotch

> Open-source web-based API client for REST, GraphQL, WebSocket, and more.

**Platforms:** macOS, Linux, Windows (web-based + self-hostable)

## Links
- [Official Website](https://hoppscotch.io)
- [GitHub Repository](https://github.com/hoppscotch/hoppscotch)
- [Documentation](https://docs.hoppscotch.io)

## Install

Hoppscotch is primarily a web app — use it directly at [hoppscotch.io](https://hoppscotch.io) with no installation required.

### Self-hosted (all platforms via Docker)

All-in-one container:

```bash
docker run -p 3000:3000 -p 3100:3100 -p 3170:3170 \
  --env-file .env \
  --restart unless-stopped \
  hoppscotch/hoppscotch
```

Or use the official Docker Compose setup:

```bash
curl -O https://raw.githubusercontent.com/hoppscotch/hoppscotch/main/docker-compose.yml
# Edit .env file with your database URL, then:
docker compose up -d
```

After startup, run database migrations:

```bash
docker exec -it <container_name> npx prisma migrate deploy
```

## Alternatives
- [bruno.md](bruno.md)
- [insomnia.md](insomnia.md)
- [postman.md](postman.md)
