# Infrastructure as Code (IAC) Project using Terragrunt

This project uses Terragrunt to automate the cloud infrastructure configuration. Terragrunt is a Terraform management tool that provides an additional layer of abstraction and configuration management.

## Prerequisites

- Cloud account (AWS, Google Cloud, Azure, etc.)
- [Terraform](https://www.terraform.io/downloads.html) installation
- [Terragrunt](https://terragrunt.gruntwork.io/#install-terragrunt) installation

## How to use

1. Clone this repository to your local development environment.
2. Configure the necessary environment variables to access your cloud account (see `terraform.tfvars` file).
3. Run the `terragrunt init` command at the root of the project to download all Terraform dependencies.
4. Run the `terragrunt apply` command to apply the configurations to your cloud account.

## Project structure

The project is structured in directories, where each directory represents an infrastructure configuration. The `terragrunt.hcl` file in each directory specifies the Terraform configurations for that resource.

## Notes

- Make sure you have permission to access your cloud account before running the `terragrunt apply` command.
- Make sure the configurations in `terraform.tfvars` are according to your needs before running the `terragrunt apply` command.
