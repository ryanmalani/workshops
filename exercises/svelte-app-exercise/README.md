# Exercise

## Svelte App into UDS

### [UDS Core Docs](https://uds.defenseunicorns.com/core/)

### Completing the Exercise

In this exercise, the goal is to package an app that doesn't have a container image or helm charts.

The steps are:

1. Create a Dockerfile to build an image for the svelte application
2. Create a zarf package in `zarf.yaml`
3. Create 4 Manifests files for:
   - Deployment Parameters `deployment.yaml`
   - Namespace Definition `namespace.yaml`
   - Service Parameters `service.yaml`
   - App Integration to UDS Core `uds-package`
4. Create UDS tasks to run commands to build and deploy application `tasks.yaml`

The defined commands will be the end result, either ran via terminal or referencing `tasks.yaml`, executed with `uds run <task>`

```bash
docker build -t ghcr.io/<repo>/ui:0.0.1 .
#need to describe packaging the app. There are 2 paths 1. use tasks.yaml 2. run commands manually
```

The app can then be deployed with:

```bash
uds zarf package deploy
```
