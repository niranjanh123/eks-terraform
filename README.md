# EKS Terraform Deployment

This repository contains Terraform configurations to set up an Amazon Elastic Kubernetes Service (EKS) cluster on AWS.

## Prerequisites

Before you begin, ensure you have the following:

- **Terraform**: Installed on your local machine. Follow the [official installation guide](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) if needed.
- **AWS CLI**: Installed and configured with the necessary permissions to create EKS clusters and associated resources. Refer to the [AWS CLI installation guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) for assistance.

## Repository Structure

- `eks.tf`: Defines the EKS cluster and node group configurations.
- `vpc.tf`: Configures the Virtual Private Cloud (VPC) and its components.
- `security-groups.tf`: Sets up security groups for the cluster.
- `variables.tf`: Contains variable definitions for the Terraform configurations.
- `outputs.tf`: Specifies the outputs of the Terraform configurations.
- `versions.tf`: Specifies the required provider versions.

## Usage

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/niranjanh123/eks-terraform.git
   cd eks-terraform
   ```

2. **Initialize Terraform**:

Initialize the Terraform working directory and download the necessary providers.

```bash
terraform init
```

3. **Review and Modify Variables**:

Inspect the variables.tf file and adjust the default values as needed to fit your environment.

4. **Plan the Deployment**:

Generate and review an execution plan to understand the resources Terraform will create or modify.

```bash
terraform plan
```

5. **Apply the Configuration**:

Apply the Terraform configurations to create the EKS cluster and related resources.

```bash
terraform apply
```
