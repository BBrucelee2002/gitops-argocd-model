# GitOps Repository for Microservices

This repository follows GitOps principles to manage Kubernetes deployments for 5 microservices across development, staging, and production environments.

## Repository Structure

- `/base`: Contains the base Kubernetes manifests for each microservice
- `/environments`: Contains environment-specific overlays for each microservice
  - `/dev`: Development environment configurations
  - `/staging`: Staging environment configurations
  - `/prod`: Production environment configurations

## Usage

This repository is designed to be used with Argo CD for continuous deployment. Each change to this repository will trigger a synchronization in Argo CD, deploying changes to the appropriate environment.
