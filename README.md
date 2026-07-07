# Stackfor-fastapi

Generated with Stackform. This stack contains 4 service(s):

- **fastapi** -- `python:3.12-slim` (Application)
- **postgres** -- `postgres:16-alpine` (Database)
- **nginx** -- `nginx:1.27-alpine` (Reverse Proxy)
- **caddy** -- `caddy:2-alpine` (Reverse Proxy)

## Getting started

```bash
cp .env.example .env
docker compose up -d --build
```

## Ports

- `fastapi`: host **8000** → container **8000**
- `postgres`: host **5432** → container **5432**
- `nginx`: host **80** → container **80**
- `nginx`: host **443** → container **443**
- `caddy`: host **80** → container **80**
- `caddy`: host **443** → container **443**

## Notes

- Update placeholder passwords in `.env` before deploying.
- Named volumes persist data between restarts; remove them with `docker compose down -v` to reset.
