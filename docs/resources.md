# Resources and Data Sources

## Data Sources

- `aws_ami.app_ami`
  - Filters:
    - `name`: `bitnami-tomcat-*-x86_64-hvm-ebs-nami`
    - `virtualization-type`: `hvm`
  - Owners: `979382823631` (Bitnami)

## Resources

- `aws_instance.web`
  - `ami`: `data.aws_ami.app_ami.id`
  - `instance_type`: `t3.nano`
  - `tags`:
    - `Name`: `HelloWorld`
