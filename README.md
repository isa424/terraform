# Terraform Project

This repository contains Terraform configuration files for managing infrastructure as code.

## Structure
- `main.tf`: Main Terraform configuration file.
- `variables.tf`: Input variables for the configuration.
- `outputs.tf`: Output values from the configuration.
- `terraform.tf`: Additional Terraform settings or provider configuration.
- `terraform.tfstate`, `terraform.tfstate.backup`: State files managed by Terraform.
- `.github/workflows/terraform.yml`: GitHub Actions workflow for CI/CD automation.

## Usage
1. **Initialize Terraform**
   ```sh
   terraform init
   ```
2. **Format Check**
   ```sh
   terraform fmt -check
   ```
3. **Plan Infrastructure Changes**
   ```sh
   terraform plan
   ```
4. **Apply Changes**
   ```sh
   terraform apply
   ```

## CI/CD
- On pull requests and pushes to `main`, GitHub Actions will run Terraform commands automatically.
- See `.github/workflows/terraform.yml` for details.

## Prerequisites
- [Terraform CLI](https://www.terraform.io/downloads.html)
- Appropriate cloud provider credentials (e.g., AWS, Azure, GCP)

## Security
- Store sensitive variables and credentials securely (e.g., use GitHub Secrets for CI/CD).

## License
MIT License
