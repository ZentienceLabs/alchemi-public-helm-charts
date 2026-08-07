# Alchemi Platform — Public Helm Repository

Public Helm chart repository for the [Alchemi AI Platform](https://alchemistudio.ai).

## Add the repo

```bash
helm repo add alchemi https://zentiencelabs.github.io/alchemi-public-helm-charts
helm repo update
```

## Install

```bash
helm install alchemi-platform alchemi/alchemi-platform \
  --namespace alchemi \
  --create-namespace \
  --set global.domain=platform.yourdomain.com \
  --set admin.email=admin@yourdomain.com \
  --set license.jwt=<your-license-jwt>
```

## Charts

| Chart | Version | Description |
|---|---|---|
| alchemi-platform | 0.1.0 | Alchemi AI Platform umbrella chart |
