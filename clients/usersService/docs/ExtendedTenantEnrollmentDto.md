# OpenapiClient::ExtendedTenantEnrollmentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **user_id** | **String** |  | [optional] |
| **is_root** | **Boolean** |  | [optional] |
| **is_owner** | **Boolean** |  | [optional] |
| **is_admin** | **Boolean** |  | [optional] |
| **is_disabled** | **Boolean** |  | [optional] |
| **tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |
| **user** | [**UserDto**](UserDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExtendedTenantEnrollmentDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  user_id: null,
  is_root: null,
  is_owner: null,
  is_admin: null,
  is_disabled: null,
  tenant: null,
  user: null
)
```

