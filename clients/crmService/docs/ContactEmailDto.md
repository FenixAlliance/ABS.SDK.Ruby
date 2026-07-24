# OpenapiClient::ContactEmailDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **address** | **String** |  | [optional] |
| **label** | **String** |  | [optional] |
| **is_primary** | **Boolean** |  | [optional] |
| **is_verified** | **Boolean** |  | [optional] |
| **verified_timestamp** | **Time** |  | [optional] |
| **contact** | [**ContactDto**](ContactDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ContactEmailDto.new(
  id: null,
  timestamp: null,
  contact_id: null,
  tenant_id: null,
  enrollment_id: null,
  address: null,
  label: null,
  is_primary: null,
  is_verified: null,
  verified_timestamp: null,
  contact: null
)
```

