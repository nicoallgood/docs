---
# generated by https://github.com/hashicorp/terraform-plugin-docs
title: kestra_user
icon: /docs/icons/terraform.svg
editLink: false
description: |-
  Manages a Kestra User.
---

# kestra_user (Resource)

Manages a Kestra User.

## Example Usage

```hcl
resource "kestra_user" "example" {
  username    = "my-username"
  namespace   = "io.kestra.mynamespace"
  description = "Friendly description"
  first_name  = "John"
  last_name   = "Doe"
  email       = "john@doe.com"
  groups      = ["4by6NvSLcPXFhCj8nwbZOM"]
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `username` (String) The user name.

### Optional

- `description` (String) The user description.
- `email` (String) The user email.
- `first_name` (String) The user first name.
- `groups` (List of String) The user groups id.
- `last_name` (String) The user last name.
- `namespace` (String) The linked namespace.

### Read-Only

- `id` (String) The ID of this resource.

## Import

Import is supported using the following syntax:

```shell
terraform import kestra_user.example {{user_id}}
```
