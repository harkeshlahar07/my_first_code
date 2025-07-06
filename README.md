terraform {
  required_providers {
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "=3.0.0"
    }
  }
}

provider "azurerm" {
  features {}
  subscription_id = "57da9eea-8d43-492a-b13e-666b4c09d465"
}

resource "azurerm_resource_group" "example1" {
  name     = "example-resources2"
  location = "eastus"
}
