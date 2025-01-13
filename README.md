# Simple Python App Manifests Repository

This repository contains Kubernetes manifests for deploying the `simple-python-app` to a Kubernetes cluster. It includes the `deployment.yml`, `service.yml`, and `ingress.yml` files used for deployment, services, and ingress.

## Table of Contents
- [Simple Python App Manifests Repository](#simple-python-app-manifests-repository)
  - [Table of Contents](#table-of-contents)
  - [Prerequisites](#prerequisites)
  - [Kubernetes Manifests Overview](#kubernetes-manifests-overview)
    - [Sample `deployment.yml`](#sample-deploymentyml)
  - [ArgoCD Integration](#argocd-integration)
  - [License](#license)
  - [Credits](#credits)

## Prerequisites

Ensure you have the following:
- **Kubernetes cluster** for deploying the app.
- **ArgoCD** for continuous delivery and deployment.

## Kubernetes Manifests Overview

This repository contains the following Kubernetes manifest files:

- **`deployment.yml`**: Defines the deployment of the `simple-python-app` with Docker image specifications.
- **`service.yml`**: Exposes the app using a NodePort service for external access.
- **`ingress.yml`**: Configures an ingress resource for routing traffic to the app.

### Sample `deployment.yml`

## ArgoCD Integration

ArgoCD monitors the `deployment.yml`, `service.yml`, and `ingress.yml` manifests. Whenever the `deployment.yml` is updated with a new Docker image tag, ArgoCD automatically deploys the latest version to the Kubernetes cluster.

## License

This project is licensed under the MIT License.

## Credits

- ArgoCD for deployment automation.
- Kubernetes for container orchestration.
