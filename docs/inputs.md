# Inputs

Currently, there are no active input variables in `variables.tf`. A commented-out variable exists and can be enabled if desired.

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|----------|
| instance_type | Type of EC2 instance to provision | string | "t3.nano" | no (commented) |

To enable, uncomment in `variables.tf`:

```hcl
variable "instance_type" {
  description = "Type of EC2 instance to provision"
  default     = "t3.nano"
}
```
