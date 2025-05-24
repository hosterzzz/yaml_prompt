# Kubernetes Manifests Prompt Portfolio

This repository contains parameterized Kubernetes manifests with reusable templates.

## Manifest Catalog

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|--------|-------------|---------|
| app.yaml | `Generate a Kubernetes Deployment manifest with configurable name, replicas, container name, image, and port` | Basic deployment manifest with parameterized values for common deployment fields. | [app.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app.yaml) |
| app-livenessProbe.yaml | `Generate a Kubernetes Deployment manifest with a configurable HTTP liveness probe` | Deployment with liveness probe for container health monitoring. | [app-livenessProbe.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | `Generate a Kubernetes Deployment manifest with a configurable HTTP readiness probe` | Deployment with readiness probe to check when container is ready to accept traffic. | [app-readinessProbe.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml | `Generate a Kubernetes Deployment manifest with configurable volume mounts` | Deployment with volume mounts for container configuration or persistent storage. | [app-volumeMounts.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml | `Generate a Kubernetes CronJob manifest with configurable schedule, image, and command` | CronJob to run containers on a specified schedule. | [app-cronjob.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/yaml/app-cronjob.yaml) |
| app-job.yaml | `Generate a Kubernetes Job manifest for single execution tasks` | One-time execution job with configurable image and command. | [app-job.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-job.yaml) |
| app-multicontainer.yaml | `Generate a Kubernetes Pod manifest with multiple containers` | Pod definition running multiple containers in a single pod. | [app-multicontainer.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-multicontainer.yaml) |
| app-resources.yaml | `Generate a Kubernetes Deployment manifest with configurable resource requests and limits` | Deployment with CPU and memory resource constraints. | [app-resources.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-resources.yaml) |
| app-secret-env.yaml | `Generate a Kubernetes Deployment manifest with environment variables from secrets` | Deployment that securely injects sensitive data as environment variables. | [app-secret-env.yaml](https://github.com/hosterzzz/yaml_prompt/blob/main/yaml/app-secret-env.yaml) |

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