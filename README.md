# Kestra (Domoro)

This repository contains a minimal Docker Compose setup for running Kestra CE on a single host.

## Services
- **Kestra** UI/API: `http://localhost:8083` (internal), public via Cloudflare Access
- **Postgres**: local persistent database for Kestra metadata

## Run
```bash
cd /opt/kestra
docker compose up -d
```

## URLs
- **Public**: `https://kestra.domoro.rechl.dev` (via Cloudflare Access)
- **Local**: `http://127.0.0.1:8083` (redirects to `/ui/`)

## Notes
- SSO is enforced by Cloudflare Access (M365).
- Kestra CE does not provide built-in SSO.
