# OpenapiClient::RefundRequestCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **approved** | **Boolean** |  | [optional] |
| **approved_timestamp** | **Time** |  | [optional] |
| **support_entitlement_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **refund_policy_id** | **String** |  | [optional] |
| **payment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RefundRequestCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  approved: null,
  approved_timestamp: null,
  support_entitlement_id: null,
  contact_id: null,
  refund_policy_id: null,
  payment_id: null
)
```

