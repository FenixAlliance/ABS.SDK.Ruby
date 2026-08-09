# OpenapiClient::CrmContext

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **owner_tenant_id** | **Object** |  | [optional] |
| **owner_tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **user_contact_id** | **Object** |  | [optional] |
| **tenant_contact_id** | **Object** |  | [optional] |
| **user_contact** | [**ContactDto**](ContactDto.md) |  | [optional] |
| **tenant_contact** | [**ContactDto**](ContactDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CrmContext.new(
  owner_tenant_id: null,
  owner_tenant: null,
  user_contact_id: null,
  tenant_contact_id: null,
  user_contact: null,
  tenant_contact: null
)
```

