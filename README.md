# Deploying Highly Available Infrastructure and Jenkins Server on AWS

**ENG MohameNageeb**

## Overview
This project demonstrates the deployment and management of a highly available AWS infrastructure using Terraform. It includes:

- Multi–Availability Zone VPC setup
- EC2 Auto Scaling Groups
- Load Balancers for traffic distribution
- Secure networking (subnets, security groups)
- Jenkins CI/CD server deployment
- Integration with Prometheus and Grafana for monitoring

## Features
- Automated build and deployment pipelines with Jenkins
- Real-time monitoring and dashboards with Prometheus & Grafana
- Infrastructure as Code with Terraform for reproducibility
- High availability and fault tolerance across multiple AZs

## Getting Started

### Prerequisites
- AWS CLI configured with proper IAM permissions
- Terraform v1.5+ installed
- An EC2 key pair
- Jenkins (on EC2) with plugins installed as per `jenkins-setup/plugins.txt`

### Terraform Deployment
\`\`\`bash
cd terraform
terraform init
terraform plan
terraform apply
\`\`\`

### Jenkins Setup
- EC2 bootstrap script: `jenkins-setup/user-data.sh`
- Install plugins: `jenkins-setup/plugins.txt`
- Import example jobs from `jenkins-setup/jobs/`

### Monitoring
- Configure Prometheus using `monitoring/prometheus.yml`
- Import Grafana dashboards from `monitoring/grafana-dashboard.json`

### CI/CD
- Example Jenkins pipeline: `ci-cd/example-pipeline.groovy`

## License
MIT License