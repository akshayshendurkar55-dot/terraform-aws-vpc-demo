# Terraform AWS VPC Demo

A hands-on Infrastructure as Code (IaC) project demonstrating how to provision an AWS Virtual Private Cloud (VPC) and a public subnet using Terraform.

## Project Overview

This project explores the fundamentals of AWS networking through Terraform. It uses reusable variables and outputs to make infrastructure configuration easier to understand and manage.

## Architecture

```text
AWS
└── VPC
    └── Public Subnet
```

**Note:** Creating a public subnet alone does not guarantee internet connectivity. An Internet Gateway and an appropriate route table configuration are generally required.

## Technologies Used

* Amazon Web Services (AWS)
* Amazon VPC
* AWS Subnets
* Terraform
* AWS CLI
* Git and GitHub

## Features

* AWS provider configuration
* Custom VPC provisioning
* Public subnet provisioning
* Reusable configuration through variables
* Outputs for VPC ID and subnet ID
* Version control using Git and GitHub

## Repository Structure

```text
terraform-aws-vpc-demo/
├── .gitignore
├── .terraform.lock.hcl
├── README.md
├── main.tf
├── variables.tf
└── outputs.tf
```

## Prerequisites

* Terraform CLI
* AWS CLI
* An AWS account
* Properly configured AWS credentials and IAM permissions

Never commit AWS access keys, secret keys, or other credentials to GitHub.

## Getting Started

Clone the repository:

```bash
git clone https://github.com/akshayshendurkar55-dot/terraform-aws-vpc-demo.git
cd terraform-aws-vpc-demo
```

Initialize Terraform:

```bash
terraform init
```

Format and validate the configuration:

```bash
terraform fmt
terraform validate
```

Review the proposed infrastructure changes:

```bash
terraform plan
```

Only if you intend to create the resources and have reviewed the possible charges, run:

```bash
terraform apply
```

To inspect the configured outputs:

```bash
terraform output
```

## Cost and Cleanup

**AWS resources may incur charges depending on the resources, region, and usage.** Review the Terraform plan and AWS pricing before creating infrastructure.

When finished, verify that the resources are safe to remove and are managed by this Terraform configuration. Then review and confirm:

```bash
terraform destroy
```

Check the AWS Console and billing dashboard afterward for any remaining resources or charges.

## Learning Outcomes

* Understanding basic VPC and subnet concepts
* Defining AWS infrastructure using Terraform
* Working with Terraform variables and outputs
* Using the init, validate, plan, apply, and destroy workflow
* Practicing infrastructure cost awareness and cleanup

## Author

**Laxmikant Shendurkar**

Cloud Computing and DevOps Learning Projects
