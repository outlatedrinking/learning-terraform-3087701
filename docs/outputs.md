# Outputs

No active outputs are defined. The following outputs are present but commented out in `outputs.tf`:

- `instance_ami` — `aws_instance.web.ami`
- `instance_arn` — `aws_instance.web.arn`

To enable, uncomment in `outputs.tf`:

```hcl
output "instance_ami" {
  value = aws_instance.web.ami
}

output "instance_arn" {
  value = aws_instance.web.arn
}
```
