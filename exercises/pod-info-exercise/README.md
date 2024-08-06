# Deploying PodInfo to UDS Core

## [UDS Core Docs](https://uds.defenseunicorns.com/core/)

### Completing the Exercise

In this exercise, the goal is to package an app that has existing helm charts and images. The steps are:

1. Create a zarf package in `zarf.yaml`
2. Create a UDS Bundle (integrates app into UDS Core) in `uds-package.yaml`
3. The helm charts and images can be found here https://github.com/stefanprodan/podinfo
4. The ends state is to run the follow commands and be able to access the Pod Info app in the browser with the url `podinfo.uds.dev`

```bash
uds run deploy
uds zarf package create
uds zarf package deploy
```
