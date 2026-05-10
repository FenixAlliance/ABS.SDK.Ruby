# OpenapiClient::RefundRequestUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **approved** | **Boolean** |  | [optional] |
| **approved_timestamp** | **Time** |  | [optional] |
| **support_entitlement_id** | **String** |  | [optional] |
| **refund_policy_id** | **String** |  | [optional] |
| **payment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RefundRequestUpdateDto.new(
  title: null,
  description: null,
  approved: null,
  approved_timestamp: null,
  support_entitlement_id: null,
  refund_policy_id: null,
  payment_id: null
)
```

