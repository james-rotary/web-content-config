# web-content-config

Argo CD configuration repo for the Web Content API.

Pattern:
- `base/` – namespace, migration PreSync job, deployment, service.
- `overlays/dev/` – image tag & replica patches.

Uses its own logical database `web_content_db` (created by infra bootstrap job). Migrations run via job before rollout.