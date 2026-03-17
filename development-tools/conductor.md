# Conductor

> Microservices and workflow orchestration engine originally built by Netflix.

**Platforms:** macOS, Linux, Windows

## Links
- [Official Website](https://conductor-oss.org/)
- [GitHub Repository](https://github.com/conductor-oss/conductor) ⭐ 18.4k

## Install

### macOS / Linux / Windows (Docker)

```bash
docker run --init -p 8080:8080 -p 1234:5000 conductoross/conductor-standalone:3.15.0
```

The API will be available at `http://localhost:8080/api` and the UI at `http://localhost:1234`.

### From source

Requires JDK 17+.

```bash
git clone https://github.com/conductor-oss/conductor.git
cd conductor
./gradlew bootRun
```

## Alternatives
- [Docker](docker.md)
- [Portainer](portainer.md)
