# Deploying Svelte App into UDS Core

### [UDS Core Docs](https://uds.defenseunicorns.com/core/)

### Prerequisite:

- UDS Core Deployed and Running

### Zarf Package and Deploy Svelte App

```bash
uds run build-ui-image
uds run package-ui
uds zarf package deploy
```
