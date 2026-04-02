# OCI Charts

This repository stores reusable Helm charts published to `ghcr.io/x-evor`.

## Layout

- `apps/app-service`: reusable runtime chart for application services
- `infra/platform/k3s`: platform composition chart for `caddy`, `apisix`, and `vault`
- `postgresql`: PostgreSQL service chart with optional `stunnel` server/client
- `observability`: observability composition chart for server and agent components

## Release Model

- Registry: `oci://ghcr.io/x-evor`
- Each chart is versioned independently
- Runtime image tags are managed by GitOps values rather than chart versions
