# Position Pal Chat Service Helm Chart

This is a Helm chart for deploying the Position Pal Location Service. The chart includes all necessary configurations and dependencies to run the service in a Kubernetes environment.

## Configure the Chart

For a complete list of configuration options, please refer to the `values.yaml` file in the chart directory. Below are some common configurations you may want to customize:

- `image.repository`: The Docker image repository for the location service.
- `image.tag`: The Docker image tag for the location service.
- `replicaNumber`: The number of replicas for the location service deployment.
- `requiredContactPointNr`: The port on which the service will be exposed.
- `managementPort`: Akka management port
- `httpPort`: The HTTP port for the location service.
- `grpcPort`: The gRPC port for the location service.
- `akkaLicenseKey`: The License key for Akka.
- `mapboxApi`: The Mapbox API key for the location service.
  

## Install the Chart
To install the chart with the release name `my-release`:

```bash
helm install my-release . --namespace position-pal --create-namespace
```
