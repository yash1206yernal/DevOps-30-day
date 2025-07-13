# DevOps-30-day
my learning journey


# DevOps 30-Day Mastery Journey 🚀

## 📌 Overview

This repository documents my hands-on journey through a comprehensive **30-Day DevOps Mastery Plan**. Each day focuses on key DevOps concepts with practical implementations, building from foundational skills to advanced infrastructure automation. As an AWS-certified professional transitioning to DevOps, this structured learning path helped me bridge the gap between theoretical knowledge and practical implementation.

**Key Objectives:**
- Master core DevOps tools and practices
- Implement infrastructure as code (IaC) with Terraform
- Build CI/CD pipelines with GitHub Actions
- Containerize applications with Docker
- Orchestrate containers with Kubernetes
- Implement monitoring with Prometheus and Grafana

## 🛠️ Core Projects

### 1. Infrastructure as Code with Terraform
- Provisioned AWS resources (EC2, VPC, S3)
- Implemented reusable Terraform modules
- Configured remote state management in S3

```bash
cd terraform-aws-infra/basic-ec2
terraform init
terraform plan
terraform apply

2. CI/CD Pipeline with GitHub Actions
Location: /github-actions-pipelines
Automated build and test workflows
Containerized application deployment
Docker image publishing to registry

yaml
name: Node.js CI/CD
on: [push]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v3
    - name: Build Docker image
      run: docker build -t myapp:${{ github.sha }} .
    - name: Push to Docker Hub
      uses: docker/build-push-action@v2
      with:
        username: ${{ secrets.DOCKER_USERNAME }}
        password: ${{ secrets.DOCKER_PASSWORD }}

3. Kubernetes Deployment

Managed deployments and services
Configured Helm charts
Implemented health checks and scaling

# Apply Kubernetes manifests
kubectl apply -f deployment.yaml

# Install Helm chart
helm install myapp ./helm-chart

# Verify deployment
kubectl get pods

4. Monitoring Stack

Prometheus configuration for metric collection
Grafana dashboards for visualization
Alert rule configurations

🚀 Getting Started
Clone the repository:

bash
git clone https://github.com/yash1206yernal/DevOps-30-day.git
cd DevOps-30-day

Prerequisites:

AWS Account (Free Tier)
Terraform v1.2+
Docker Desktop
Kubernetes (Minikube or kind)
GitHub Account

📜 Certifications Earned
Certification	Status	Verification
AWS Solutions Architect Professional	✅ https://www.credly.com/badges/4290626f-91c8-4754-8789-8e8b9b78e70b
AWS Solutions Architect Associate	✅	https://www.credly.com/badges/dee5ef69-810b-4631-94c5-1ff95c1a5dfc
AWS Cloud Practitioner	✅	https://www.credly.com/badges/32777f0c-163d-4113-9cbc-778c03a199b0
Terraform Associate	In Progress	-
Kubernetes (CKAD)	Planned	-
