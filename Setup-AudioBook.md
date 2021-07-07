---
title: Setup Terraform
tags: ['Terraform', 'Terraform Setup', 'AudioBook']
---

# Prerequisites
- The Terraform CLI (0.14.9+) installed.
    - https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/aws-get-started
    - Check terraform version
    ```bash
    terraform --version
    ```

- The AWS CLI installed.
    - https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html
- AWS account.
- Your AWS credentials.
    - Config aws credentials
    ```bash
    aws configure --profile audiobook
    ```
    
    -  check aws config
    ```bash
    aws configure list --profile audiobook
    ```
----
**NOTE**
The configuration process stores your credentials in a file at `~/.aws/credentials` on MacOS and Linux, or `%UserProfile%\.aws\credentials` on Windows.
----



# How to install
## Init terraform
```bash
terraform init
```

## Validate terraform config
```bash
terraform validate
```

## Check plan change
```bash
terraform plan
```

## Apply change
```bash
terraform apply
```

## Destroy
```bash
terraform destroy
```
 
Ref: https://learn.hashicorp.com/tutorials/terraform/infrastructure-as-code?in=terraform/aws-get-started
