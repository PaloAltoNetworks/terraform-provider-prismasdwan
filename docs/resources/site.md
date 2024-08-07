---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "prismasdwan_site Resource - prismasdwan"
subcategory: ""
description: |-
  Manages a Prisma SD-WAN site.
---

# prismasdwan_site (Resource)

Manages a Prisma SD-WAN site.

## Example Usage

```terraform
resource "prismasdwan_site" "example" {
  config = "/Users/jdoe/sdwan_configs/site1.json"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `config` (String) The filesystem path of the site's JSON config.

### Optional

- `is_deployed` (Boolean) This will be set to false if the site config deployed does not match the given config file.
- `timeout` (String) Timeouts for this resource's operations. A custom timeout is a string that has a number and a units suffix, such as 30s or 1h1m1s. Valid units are "h", "m", or "s". Note that changes to custom timeouts only take effect during resource creation or update. Default: 30m.

### Read-Only

- `id` (String) Unique identifier for this resource.
- `tfid` (String) The Terraform ID for this resource.
