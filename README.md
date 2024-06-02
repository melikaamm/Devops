# Devops
# Project Concept for DevOps Deployment of a TODO Application

## Application Lifecycle and Technology Stack

The application chosen for this DevOps project is a Dockerized TODO app that utilizes MongoDB for its primary database. The entire lifecycle of the application, from development to deployment, will be automated using various DevOps tools and practices.

### Technology Stack

- **Docker**: Containerizes the TODO application for consistent environments across different stages.
- **MongoDB**: Primary database for storing TODO items.
- **Terraform**: Infrastructure as Code (IaC) for provisioning and managing AWS resources.
- **GitHub Actions**: CI/CD pipeline for automating build, test, and deployment processes.
- **AWS CloudWatch and Prometheus**: Monitoring and logging to track application performance and health.

## Application Lifecycle

1. **Development**: 
   - Code is written and version-controlled in a Git repository.
   - Docker is used to containerize the application, ensuring consistent environments across different stages.

2. **Build and Test**:
   - GitHub Actions triggers automated builds and tests whenever code is pushed to the repository.
   - Docker images are built and tested to ensure the application runs correctly in the container.

3. **Deployment**:
   - Terraform is used to provision the necessary AWS infrastructure.
   - GitHub Actions deploys the Docker images to Amazon ECS.
   - The application is made accessible via an Application Load Balancer.

4. **Monitoring and Maintenance**:
   - AWS CloudWatch and Prometheus monitor application performance and health.
   - Alerts are set up for any anomalies or performance issues.

## Architecture and Infrastructure Provisioning

### Infrastructure Components

- **Amazon ECS (Elastic Container Service)**: Runs the Dockerized TODO application.
- **Amazon DocumentDB**: MongoDB-compatible database service for storing TODO items.
- **Amazon S3 (Simple Storage Service)**: Stores static files.
- **Amazon CloudWatch and AWS X-Ray**: Provides monitoring and logging capabilities.
- **VPC (Virtual Private Cloud)**: Isolates application infrastructure with separate subnets for different tiers.
- **Application Load Balancer (ALB)**: Distributes traffic across ECS containers.
- **Security Groups**: Controls inbound and outbound traffic to resources.

### Provisioning with Terraform

- **Terraform** scripts define the entire infrastructure setup.
- **Version-controlled** configuration files ensure reproducibility and collaboration.
- **Automated provisioning** enables consistent and scalable environments.

## Decision Rationale

### Terraform for Provisioning

- **Declarative Configuration**: Manages complex infrastructure setups.
- **Version Control**: Ensures consistent environments and collaboration.
- **Scalability**: Easily replicates environments and scales infrastructure.

### GitHub Actions for CI/CD

- **Integration**: Seamlessly integrates with GitHub repositories.
- **Automation**: Efficiently automates build, test, and deployment processes.

### AWS Services

- **Managed Services**: Reduces operational burden, allowing focus on application development.
- **Reliability and Scalability**: Ensures high performance and availability.
- **Monitoring**: CloudWatch and Prometheus provide comprehensive monitoring and alerting capabilities.

## Summary

This project leverages a robust and scalable AWS infrastructure, managed via Terraform, with a streamlined CI/CD pipeline using GitHub Actions, and comprehensive monitoring to ensure the application's reliability and performance. This setup not only meets the project's technical requirements but also provides a solid foundation for future scalability and maintenance.

## Repository Link

The project files are stored and tracked in the following Git repository: [Git Repository Deep Link](https://your-git-repository-link)

---

Melika Amirkhalili
