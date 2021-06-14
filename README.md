# terraform_march_azure

## Creates Three-Tier Terraform on Azure

```
# needs to create backend.tf

backend.tf filels inside:

terraform {
  backend "azurerm" {
    resource_group_name  = "Dev"
    storage_account_name = "backendmiradil"
    container_name       = "backend"
    access_key           = "copy from console Home >> Storage Account >> Access keys"
    key                  = "dev_terraform.tfstate"
  }
}



```
