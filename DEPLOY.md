# redesign https://outsmartpest.com using an up to d (Fork) — Deployment Guide

## Deploy with Starlight Hyperlift (Recommended)

1. Push this repo to GitHub
2. Go to [spaceship.com/starlight-cloud/hyperlift](https://www.spaceship.com/starlight-cloud/hyperlift/)
3. Connect your GitHub repository
4. Hyperlift auto-deploys on every push — **no other config needed**

> The `Dockerfile` in this repo root is all Hyperlift needs.

## Deploy with Docker (Self-hosted)

```bash
docker build -t redesign https://outsmartpest.com using an up to d (Fork) .
docker run -p 80:80 redesign https://outsmartpest.com using an up to d (Fork)
```

## Deploy with Docker Compose

```bash
docker compose up -d
```

## Deploy to cPanel / Shared Hosting (HTML only)

Upload the contents of this folder to your `public_html` directory via FTP or cPanel File Manager.
