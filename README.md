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

### 2. `main.tf` 
- **Purpose**: Defines the overall infrastructure resources.
- **Why**: Acts as the entry point for Terraform configurations. 

### 3. `variables.tf`
- **Purpose**: Declares variables used across the configuration.
- **Why**: Makes the configuration dynamic and easier to manage. 

### 4. `outputs.tf`
- **Purpose**: Specifies the outputs to display key information about the infrastructure.
- **Why**: Useful for displaying important details about the deployed infrastructure.

### 5. `ec2.tf & s3.tf`
- **Purpose**: Configures the provisioning of EC2 instances & management of s3.
- **Why**: Essential for creating and managing EC2 instances as well as s3 in AWS.

### 6. `dynamodb.tf` 
- **Purpose**: Configures DynamoDB tables for NoSQL database solutions.
- **Why**: Useful for creating and managing DynamoDB tables for NoSQL database needs. 


## Key Features
	-	Infrastructure as Code (IaC): Automates infrastructure management with code.
	-	Modularity: Reusable modules for scalable infrastructure provisioning.
	-	AWS Resource Management: Examples for provisioning EC2, S3, and DynamoDB resources.
	-	Parameterization: Dynamic configurations using variables.
	-	Output Management: Easily retrieve essential information about deployed resources.
	-	State Tracking: Uses state files to track the current state of the infrastructure.

  