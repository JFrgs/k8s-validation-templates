# Network Apps Integration and Deployment

This repository contains the necessary information and instructions (manifest files) for integrating and deploying Network Apps within the Athens K8s Cluster. The integration activities aim to validate the Network Applications, showcasing their validation when integrated with the vApp.

## Goals of Deployment Activities

The deployment activities focus on achieving the following goals:

1. Integration of 5G Connectivity: Validate the real 5G connectivity for each specific use case (whether it is applicable)
2. Ensure Effective Communication: Establish communication channels between the vApp, Network Application, NEF, CAPIF, and TSN.

## Versioning

| Component | Version   |
|-----------|-----------|
| CAPIF     | v3.1.2    |
| NEF       | v2.2.2    |
| SDK       | v1.0.7    |
| TSN       | v1.2.1    |

## Kubernetes Cluster

This repository is organized as follows:

- `nginx-manifests`: Includes the manifest to set up the Nginx Ingress Controller. Through ingress rules (hostnames), it forwards incoming requests to the K8s services and subsequently to the respective pods where the containers reside.
- `MetalLB`: Provides the required resources for MetalLB, which assigns an external IP address to the Nginx Ingress Controller. This enables accessibility within the NCSRD infrastructure. (through VPN)

