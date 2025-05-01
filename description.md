# VPC Terraform Setup

This document provides a detailed description of the VPC setup using Terraform.

## Overview

The purpose of this setup is to provision and manage a Virtual Private Cloud (VPC) infrastructure using Terraform. This includes subnets, route tables, internet gateways, and other necessary components.

## Features

- Creation of a VPC with customizable CIDR blocks.
- Support for public and private subnets.
- Internet Gateway and NAT Gateway configuration.
- Route tables and route associations.
- Security groups for access control.

## Prerequisites

- Terraform installed on your local machine.
- AWS CLI configured with appropriate credentials.
- Basic understanding of Terraform and AWS networking.

## Usage

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd vpc-terraform-setup
    ```

2. Initialize Terraform:
    ```bash
    terraform init
    ```

3. Review and update `variables.tf` as needed.

4. Apply the configuration:
    ```bash
    terraform apply
    ```

5. Confirm the changes and wait for the resources to be provisioned.

## Notes

- Ensure that the AWS region is correctly set in the provider configuration.
- Review the Terraform state file for any sensitive information.

## Cleanup

To destroy the created resources, run:
```bash
terraform destroy
```

## References

- [Terraform Documentation](https://www.terraform.io/docs)
- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc)
