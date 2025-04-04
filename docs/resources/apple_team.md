---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "eas_apple_team Resource - terraform-provider-eas"
subcategory: ""
description: |-
  
---

# eas_apple_team (Resource)



## Example Usage

```terraform
terraform {
  required_providers {
    eas = {
      source  = "fintreal/eas"
      version = "~> 1.4"
    }
  }
}

provider "eas" {}

resource "eas_apple_team" "eas_apple_team" {
  identifier = "TEST_APPLE_TEAM_ID"
  type       = "COMPANY_OR_ORGANIZATION"
  name       = "Test Team"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `identifier` (String) The identifier of the Apple Team
- `name` (String) The name of the Apple Team
- `type` (String) Apple Team type. Can be `COMPANY_OR_ORGANIZATION`, `IN_HOUSE` or `INDIVIDUAL`.

### Read-Only

- `id` (String) The ID of the Apple Team
