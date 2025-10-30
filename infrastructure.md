Terraform/K8s setup, CI/CD pipelines, environment variables, secrets, deployment flow, scaling/monitoring

# OrtemHealth Infrastructure Documentation

## Overview
OrtemHealth infrastructure is fully cloud-native, supporting easy deployment, scaling, and monitoring via AWS, Terraform, Kubernetes, and CI/CD automation.

## Key Components

- **Infrastructure as Code (IaC):**  
  - `terraform/`: AWS VPC, subnet, RDS/EC2 configs
  - K8s manifests for services, autoscaling, health checks
  - S3 remote state for Terraform

- **CI/CD Pipelines**
  - GitHub Actions: `/infrastructure/.github/workflows/deploy.yml`
  - Steps for build, test, Docker push, Terraform apply, K8s deploy

- **Secrets and Environment Management**
  - GitHub Secrets for AWS and DB keys
  - `.env.example` files per service

- **Monitoring and Logging**
  - Prometheus and Grafana for backend metrics
  - Sentry for app error tracking
  - Health endpoints for all microservices

## Quickstart

1. Install Terraform and AWS CLI
2. Run `terraform init` and `terraform plan` inside `infrastructure/terraform` for new environments
3. Use `docker-compose.yml` (local dev) or deploy Docker images to K8s via CI/CD

## Scaling & Reliability

- Horizontal pod autoscaling via K8s
- Cloud DB backup via AWS RDS
- Blue/green deploy strategy via CI/CD

## Troubleshooting

- All builds and deploys logged in GitHub Actions
- Monitor K8s pods with `kubectl get pods -A`

