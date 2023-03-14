# chart

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.1.0](https://img.shields.io/badge/AppVersion-0.1.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| configLogging.Example | string | see [values.yaml](values.yaml) |  |
| configObservability.Example | string | see [values.yaml](values.yaml) |  |
| knativeOperator.knativeOperator.env.configLoggingName | string | `"config-logging"` |  |
| knativeOperator.knativeOperator.env.configObservabilityName | string | `"config-observability"` |  |
| knativeOperator.knativeOperator.env.metricsDomain | string | `"knative.dev/operator"` |  |
| knativeOperator.knativeOperator.image.repository | string | `"gcr.io/knative-releases/knative.dev/operator/cmd/operator@sha256"` |  |
| knativeOperator.knativeOperator.image.tag | string | `"2e73ab904a74aa6c6ed1b8fe6f46d14444918bf486ab5bb0febdb2fbc77aa033"` |  |
| knativeOperator.replicas | int | `1` |  |
| kubernetesClusterDomain | string | `"cluster.local"` |  |
| operatorWebhook.operatorWebhook.env.configLoggingName | string | `"config-logging"` |  |
| operatorWebhook.operatorWebhook.env.configObservabilityName | string | `"config-observability"` |  |
| operatorWebhook.operatorWebhook.env.metricsDomain | string | `"knative.dev/operator"` |  |
| operatorWebhook.operatorWebhook.env.webhookName | string | `"operator-webhook"` |  |
| operatorWebhook.operatorWebhook.env.webhookPort | string | `"8443"` |  |
| operatorWebhook.operatorWebhook.image.repository | string | `"gcr.io/knative-releases/knative.dev/operator/cmd/webhook@sha256"` |  |
| operatorWebhook.operatorWebhook.image.tag | string | `"3d827626e563b24b8c001424d48bf8f07725223a07d0478148f3c021b4e9e647"` |  |
| operatorWebhook.operatorWebhook.resources.limits.cpu | string | `"500m"` |  |
| operatorWebhook.operatorWebhook.resources.limits.memory | string | `"500Mi"` |  |
| operatorWebhook.operatorWebhook.resources.requests.cpu | string | `"100m"` |  |
| operatorWebhook.operatorWebhook.resources.requests.memory | string | `"100Mi"` |  |
| operatorWebhook.ports[0].name | string | `"http-metrics"` |  |
| operatorWebhook.ports[0].port | int | `9090` |  |
| operatorWebhook.ports[0].targetPort | int | `9090` |  |
| operatorWebhook.ports[1].name | string | `"http-profiling"` |  |
| operatorWebhook.ports[1].port | int | `8008` |  |
| operatorWebhook.ports[1].targetPort | int | `8008` |  |
| operatorWebhook.ports[2].name | string | `"https-webhook"` |  |
| operatorWebhook.ports[2].port | int | `443` |  |
| operatorWebhook.ports[2].targetPort | int | `8443` |  |
| operatorWebhook.type | string | `"ClusterIP"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)