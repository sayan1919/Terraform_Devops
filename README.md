# Terraform for DevOps

A comprehensive repository to help DevOps engineers automate infrastructure deployments using Terraform. This repository focuses on managing AWS resources like EC2 instances, S3 buckets, and DynamoDB tables with best practices in Infrastructure as Code (IaC).

---

## Project Structure

The project is organized into multiple files and directories to ensure scalability, reusability, and maintainability.

### Main Files:
- **`main.tf`**: The entry point for defining overall infrastructure resources.
- **`variables.tf`**: Declares all variables used across the configuration to make it dynamic.
- **`outputs.tf`**: Specifies the outputs to display key information about the infrastructure.
- **`provider.tf`**: Configures the AWS provider with authentication and region details.

### Additional Files:
- **`ec2.tf`**: Contains the configuration for provisioning EC2 instances.
- **`s3.tf`**: Manages the configuration for creating and managing S3 buckets.
- **`dynamodb.tf`**: Configures DynamoDB tables for NoSQL database solutions.
- **`terraform.tfvars`**: Provides values to the variables declared in `variables.tf`.

### State and Backend Files:
- **`terraform.tfstate`**: Tracks the current state of the infrastructure managed by Terraform.
- **`terraform.tfstate.backup`**: A backup of the previous state to ensure safety.

### Directories:
- **`aws_module_project/`**: Contains reusable modules for managing AWS resources.
- **`modules/`**: Houses modular Terraform configurations that can be reused across multiple projects.

---

## File Details and Purpose

### 1. `provider.tf`
- **Purpose**: Specifies the cloud provider (AWS) and its credentials.
- **Why**: Required for Terraform to authenticate with AWS and manage resources.
- **Example**:
  ```hcl
  provider "aws" {
    region     = "us-west-1"
    access_key = "your_access_key"
    secret_key = "your_secret_key"
  } 
