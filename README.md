# rexec-stack Helm Chart Repository

Public Helm chart repository for the SciDx Rexec Stack, hosted via GitHub Pages.

## Usage

### Add the Helm repository

```bash
helm repo add rexec-stack https://thomhford.github.io/helm-repo/
helm repo update
```

### Search available charts

```bash
helm search repo rexec-stack
```

### Install the chart

```bash
helm install rexec rexec-stack/rexec-stack -n rexec --create-namespace
```

### Install with custom values

```bash
helm install rexec rexec-stack/rexec-stack -n rexec --create-namespace -f my-values.yaml
```

## Chart Components

- **rexec-broker**: SciDx Remote Execution broker
- **rexec-server-deployment-api**: Rexec Server Deployment API
- **ndp-ep-api**: NDP Endpoint API (disabled by default)

## Configuration

See the chart's default `values.yaml` for all configurable parameters:

```bash
helm show values rexec-stack/rexec-stack
```
