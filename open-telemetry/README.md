# Open Telemetry

## Helm Repository

```sh
helm repo add open-telemetry https://open-telemetry.github.io/opentelemetry-helm-charts

helm repo update
```

## Collector

[Collector](https://opentelemetry.io/docs/kubernetes/helm/collector/)

```sh
helm upgrade --install \
   --namespace opentelemetry --create-namespace \
   --values=./values.yaml \
   opentelemetry-collector open-telemetry/opentelemetry-collector
```
