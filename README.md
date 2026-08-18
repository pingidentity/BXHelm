# Ping Identity BX Helm Charts

This repository contains the Ping Identity Helm charts used for deploying Ping Identity BX demos and products with Helm.

This chart includes the Ping Identity DevOps Helm chart as a child dependency.

The complete collection of documentation for our Helm charts and other resources is located [here](https://helm.pingidentity.com).

See [Ping Identity's DevOps Page](https://devops.pingidentity.com) for additional resources.

### Useful Helm commands

Add the Ping BX chart repo:

```helm repo add ping-bx https://pingidentity.github.io/BXHelm```

Download the chart locally:

```helm pull ping-bx/ping-bx --untar```

Update the chart package. Be sure to increment the version in the Chart.yaml.

```helm package charts/ping-bx```

Update the repo index after making any changes. 

```helm repo index . --url https://pingidentity.github.io/BXHelm/```
