# Helm Charts Repository

This repository contains a collection of Helm charts for deploying applications on Kubernetes. Helm is a package manager for Kubernetes that simplifies the process of defining, installing, and managing Kubernetes applications.

## Prerequisites

Before you can use the charts in this repository, you need to have Helm installed. If you haven't already installed Helm, please refer to [Helm's documentation](https://helm.sh/docs) for instructions on getting started.

## Adding the Repository

To use the charts in this repository, you need to add it as a Helm repository. Follow these steps to add the repository:

```bash
helm repo add <alias> https://github.com/firefighters-sre/helm-charts/
```

If you have previously added this repository and want to update the list of available packages, run the following command:

```bash
helm repo update
```

You can now search for charts in this repository using the following command:

```bash
helm search repo <alias>
```
## Installing a Chart
To install a specific chart from this repository, you can use the helm install command. Replace <chart-name> with the name of the chart you want to install and <alias> with the alias you used when adding the repository. For example:

```bash
helm install my-<chart-name> <alias>/<chart-name>
```
This command will deploy the chart with the specified name (my-<chart-name>) in your Kubernetes cluster.

## Uninstalling a Chart
To uninstall a chart that you've previously installed, you can use the helm delete command. Replace <chart-name> with the name of the chart you want to uninstall. For example:

```bash
helm delete my-<chart-name>
```

This will remove the chart and its resources from your Kubernetes cluster.

For more information on using Helm and Helm charts, please refer to Helm's documentation.

Happy Helm Chart deploying!