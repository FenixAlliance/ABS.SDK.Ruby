# OpenapiClient::ExtendedInviteDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **revoked** | **Boolean** |  | [optional] |
| **redeemed** | **Boolean** |  | [optional] |
| **redeemed_timestamp** | **Time** |  | [optional] |
| **user_email** | **String** |  | [optional] |
| **creator_enrollment_id** | **String** |  | [optional] |
| **related_enrollment_id** | **String** |  | [optional] |
| **tenant** | [**TenantDto**](TenantDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ExtendedInviteDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  revoked: null,
  redeemed: null,
  redeemed_timestamp: null,
  user_email: null,
  creator_enrollment_id: null,
  related_enrollment_id: null,
  tenant: null
)
```

