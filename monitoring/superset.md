# Apache Superset

> Modern data exploration and visualization platform for creating interactive dashboards.

**Platforms:** macOS, Linux, Windows (via Docker)

## Links
- [Official Website](https://superset.apache.org/)
- [GitHub Repository](https://github.com/apache/superset) ⭐ 71.0k

## Install

### macOS / Linux (Docker Compose)

```bash
git clone https://github.com/apache/superset.git
cd superset
docker compose -f docker-compose-non-dev.yml pull
docker compose -f docker-compose-non-dev.yml up
```

### macOS (pip)

```bash
pip install apache-superset
superset db upgrade
superset fab create-admin
superset init
superset run -p 8088 --with-threads --reload --debugger
```

## Alternatives
- [Grafana](grafana.md)
- [Netdata](netdata.md)
