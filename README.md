# DevOps Practical Task WebApplication

This repository contains the solution for a DevOps practical task to assess skills and expertise in the DevOps lifecycle. The task involved setting up both **Build** and **Release ** pipelines, creating Docker images, generating Helm charts, and deploying Kubernetes.

## Project Overview

The main goal of this task was to build a CI/CD pipeline in **Azure DevOps** that handles the following:

1. **Source Code Checkout**: Using `checkout: self` to retrieve the project's latest version.
2. **Docker Image Build**: Building the Docker image using the provided **Dockerfile** and pushing it to **Docker Hub**.
3. **Helm Chart Generation**: Creating Helm charts for Kubernetes deployments.
4. **Release Pipeline**: Deploy the application to Kubernetes environments (Dev and Prod) using Helm, with environment-specific configurations.

## Project Structure

Here’s the project structure:
├── CD.yml ├── CI.yml ├── Dockerfile ├── k8s │ └── deploy.yaml └── webapp ├── Chart.yaml ├── environment │ ├── deployment_dev.yaml │ ├── deployment_prod.yaml │ ├── values_dev.yaml │ └── values_prod.yaml ├── templates │ ├── deployment.yaml │ ├── hpa.yaml │ ├── ingress.yaml │ ├── service.yaml │ ├── serviceaccount.yaml │ └── tests │ └── test-connection.yaml └── values.yaml                 

## Key Features

- **CI/CD Pipelines**: Configured using Azure DevOps with `checkout: self` for code retrieval.
- **Docker & Kubernetes**: Docker image build and Kubernetes deployment via Helm.
- **Environment-Specific Configurations**: Separate configurations for **Dev** and **Prod** environments using Helm chart values.

## How to Run

1. Clone the repository.
2. Set up your Azure DevOps account and pipelines (Build and Release).
3. Configure your Kubernetes cluster.
4. Run the pipelines to build and deploy the application.

## Technologies Used

- **Azure DevOps**: For pipeline management.
- **Docker**: For containerization.
- **Helm**: For Kubernetes deployments.
- **Kubernetes**: For orchestrating the deployment.
