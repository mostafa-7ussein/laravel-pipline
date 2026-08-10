# Laravel Pipeline — Docker & Kubernetes Lab

Laravel application packaged with Docker and prepared for deployment using Compose, Ansible, and Kubernetes manifests.

## What this shows

- Containerizing a **Laravel / PHP** app with Docker
- Local/multi-service setup with **Docker Compose**
- Configuration automation with **Ansible** playbooks
- Kubernetes manifests for app, database, and phpMyAdmin

## Key files

- `Dockerfile` / `docker-compose.yml`
- `playbook.yml` / `playbook-dcompose.yml`
- `*-deployment.yaml` / `*-service.yaml` — Kubernetes resources
- `check_installations.sh` / `install.sh` — setup helpers

## Typical flow

```text
Build image → Compose or Ansible deploy → Optional Kubernetes apply
```

## Notes

- Copy `.env.example` to `.env` and set local values before running
- Do not commit production secrets
- Useful as a DevOps practice repo for PHP app delivery
