# Terraform Module Documentation

This module provisions a simple AWS EC2 instance using the most recent Bitnami Tomcat AMI.

- Data sources: `aws_ami.app_ami`
- Resources: `aws_instance.web`
- Provider: `aws`

## Usage

```hcl
terraform {
  required_providers {
    aws = {
      source = "hashicorp/aws"
    }
  }
}

provider "aws" {
  region = "us-west-2"
}

module "web_instance" {
  source = "./path-to-this-module"
  # instance_type = "t3.nano" # if variable is enabled
}
```

## Notes
- The AMI owner is Bitnami (`979382823631`).
- The instance is tagged `Name = "HelloWorld"`.
- Default `instance_type` in the module code is `t3.nano`.

See `docs/inputs.md`, `docs/outputs.md`, `docs/providers.md`, and `docs/resources.md` for details.
