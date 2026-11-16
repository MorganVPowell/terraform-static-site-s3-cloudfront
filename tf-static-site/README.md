# Terraform Static Website (S3 + CloudFront)

Infrastructure as Code version of my static website project: a private S3 bucket served over HTTPS through CloudFront with Origin Access Control, defined in Terraform and validated by a GitHub Actions pipeline.

## Architecture
(add draw.io diagram here)

## Usage
terraform init
terraform plan
terraform apply
terraform destroy   # clean up when finished

## CI/CD
GitHub Actions runs terraform fmt, init and validate on every pull request and push to main. An optional job syncs the site to S3 and invalidates the CloudFront cache.

## Issues hit and fixes
(add your own errors and fixes here)
