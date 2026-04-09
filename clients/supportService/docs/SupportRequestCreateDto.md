# OpenapiClient::SupportRequestCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **approved** | **Boolean** |  | [optional] |
| **approved_timestamp** | **Time** |  | [optional] |
| **business_id** | **String** |  | [optional] |
| **business_profile_record_id** | **String** |  | [optional] |
| **support_entitlement_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **account_holder_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SupportRequestCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  approved: null,
  approved_timestamp: null,
  business_id: null,
  business_profile_record_id: null,
  support_entitlement_id: null,
  contact_id: null,
  account_holder_id: null
)
```

