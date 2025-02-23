# Azure Container Apps Demo
This is a demo for deploying multiple containers (frontend UI container and backend redis container) within the same Azure Container App.
> Note: This example does not use Dapr.

## Overview

`Azure Container Apps` is a fully managed serverless container service that scales dynamically based on HTTP traffic or events. Container Apps enables you to enjoy the benefits of running cloud native containerized applications while leaving behind the concerns of managing cloud infrastructure and complex container orchestrators like `Kubernetes`.

>  `Azure Container Apps` is a preview service, and only available in these locations - `northcentralusstage,westcentralus,eastus,westeurope,jioindiawest,northeurope,canadacentral`

With Azure Container Apps, you can:

- Run multiple container revisions and manage the container app's application lifecycle.

- Autoscale your apps based on any KEDA-supported scale trigger. Most applications can scale to zero1.

- Enable HTTPS ingress without having to manage other Azure infrastructure.

- Split traffic across multiple versions of an application for Blue/Green deployments and A/B testing scenarios.

- Use internal ingress and service discovery for secure internal-only endpoints with built-in DNS-based service discovery.

- Build microservices with Dapr and access its rich set of APIs.

- Run containers from any registry, public or private, including Docker Hub and Azure Container Registry (ACR).

- Use the Azure CLI extension or ARM templates to manage your applications.

- Securely manage secrets directly in your application.

- View application logs using Azure Log Analytics.

## Prerequisites

- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli).
- Install the Azure Container Apps extension to the CLI
    ```sh
    az extension add -n containerapp
    ```


## Scenarios

![Azure Container Apps Example Scenarios](/docs/img/azure-container-apps-example-scenarios.png)

1. [Deploy ContainerApp with multiple containers using YAML manifest](docs/deploy-containerapp-with-multiple-containers-yaml.md)
