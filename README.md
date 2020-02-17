# Terraform AWS Lambda Layer module

## About:

AWS Lambda Layer terraform module for NodeJS 10 and 12.x programming languages.

## How to use:

```terraform
module "lambda-layer" {
  source = "github.com/rpstreef/tf-lambda-layer?ref=v1.0"

  resource_tag_name = var.resource_tag_name
  namespace         = var.namespace
  region            = var.region

  name           = local.lambda_layer_name
  zip_name       = local.lambda_layer_zip_name
  description    = local.lambda_layer_description
  
  dist_file_path = local.dist_file_path
}
```

## Changelog

### v1.0
 - Initial release

