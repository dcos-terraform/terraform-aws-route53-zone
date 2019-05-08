AWS DC/OS Route53 Zone (NOTE: THIS IS CURRENTLY EXPERIMENTAL AND NOT YET SUPPORTED)
============
This module is used to create a Route53 Zone

EXAMPLE
-------

```hcl
module "route_53_zone" {
 source                    = "dcos-terraform/route53-zone/aws"
 name                      = "testing.us"
 vpc_id                    = "vpc-123213bkjdfgab"
}
```

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| name | UNDEFINED | string | n/a | yes |
| vpc\_id | AWS VPC ID | string | `""` | no |

## Outputs

| Name | Description |
|------|-------------|
| zone\_id | ID of the Zone Created |

