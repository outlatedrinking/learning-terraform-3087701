# Providers

This module requires the AWS provider.

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
```

- **aws**: `hashicorp/aws` (version not pinned)
- Default region in example: `us-west-2`
