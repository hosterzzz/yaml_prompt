# Kubernetes Manifests Prompt Portfolio

This repository contains parameterized Kubernetes manifests with reusable templates.

## Manifest Catalog

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|--------|-------------|---------|
| app.yaml | `generate kind pod that contain 2 labels and spec ports` | Basic deployment manifest with parameterized values for common deployment fields. | [app.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app.yaml) |
| app-livenessProbe.yaml | `generate kind pod on namespace spec containers livenessProbe with initialDelaySecond, timeoutSeconds, periodSeconds, failureTrashold and ports name in yaml` | Deployment with liveness probe for container health monitoring. | [app-livenessProbe.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | `generate kind pod on namespace spec containers readinessProbe with initialDelaySecond, timeoutSeconds, periodSeconds, failureTrashold and ports name and specific path in yaml` | Deployment with readiness probe to check when container is ready to accept traffic. | [app-readinessProbe.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | `generate kind pod with ready and live probe and mount volume spec. name in yaml` | Deployment with volume mounts for container configuration or persistent storage. | [app-volumeMounts.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml | `generate kind job with spec template gce pvc and runnining command using mounted space restartpolicy never in yaml` | CronJob to run containers on a specified schedule. | [app-cronjob.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/yaml/app-cronjob.yaml) |
| app-job.yaml | `generate kind job with gce pvc and runnining command  using mounted space restartpolicy never in yaml` | One-time execution job with configurable image and command. | [app-job.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-job.yaml) |
| app-multicontainer.yaml | `generate kind pod with 2 containers that use same volume in yaml` | Pod definition running multiple containers in a single pod. | [app-multicontainer.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-multicontainer.yaml) |
| app-resources.yaml | `generate kind pod on namespace spec containers readinessProbe with initialDelaySecond, timeoutSeconds, periodSeconds, failureTrashold and ports name and specific path and resources req and limits in yaml` | Deployment with CPU and memory resource constraints. | [app-resources.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-resources.yaml) |
| app-secret-env.yaml | `generate kind pod env specify secretKeyRef and VolumeFrom secertKeyRef in yaml` | Deployment that securely injects sensitive data as environment variables. | [app-secret-env.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-secret-env.yaml) |
| app-secret.yaml | `generate kind pod that mount readonly volume with secret in yaml` | Deployment that securely injects sensitive data as environment variables. | [app-secret.yaml]
| app.yaml | `generate kind pod that contains env volume from configMapKeyRef and mount volume /config and restart policy never and imagePullPolicy - Always` | Basic deployment manifest configmap in pod. | [app.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-configmap.yaml) |

## Directory Structure

```
k8s-manifests/
├── README.md
└── yaml/
    ├── app.yaml
    ├── app-livenessProbe.yaml
    ├── app-readinessProbe.yaml
    ├── app-volumeMounts.yaml
    ├── app-cronjob.yaml
    ├── app-job.yaml
    ├── app-multicontainer.yaml
    ├── app-resources.yaml
    └── app-secret-env.yaml
```
