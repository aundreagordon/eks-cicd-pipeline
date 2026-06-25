# EKS CI/CD Pipeline

## Overview

This project demonstrates a complete CI/CD pipeline for deploying a containerized Flask application to Amazon EKS using Docker, Amazon ECR, Terraform, Helm, and Jenkins.

The application displays a simple "Hello, World!" message and is deployed to a Kubernetes cluster running on AWS EKS. Infrastructure is provisioned using Terraform, container images are stored in Amazon ECR, and application deployments are managed using Helm.

## Architecture

Application → Docker → Amazon ECR → Amazon EKS → Helm Deployment → AWS Load Balancer

## Technologies Used

* Python Flask
* Docker
* Amazon ECR
* Amazon EKS
* Terraform
* Kubernetes
* Helm
* Jenkins
* AWS IAM
* AWS VPC
* GitHub

## Project Structure

```text
eks-cicd-pipeline/
├── app/
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
├── terraform/
│   ├── provider.tf
│   ├── variables.tf
│   ├── vpc.tf
│   ├── iam.tf
│   ├── ecr.tf
│   ├── eks.tf
│   ├── ec2.tf
│   └── outputs.tf
├── helm/
│   └── hello-world/
│       ├── Chart.yaml
│       ├── values.yaml
│       └── templates/
└── README.md
```
