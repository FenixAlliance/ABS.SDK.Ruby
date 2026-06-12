# OpenapiClient::RefundRequestDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **approved** | **Boolean** |  | [optional] |
| **approved_timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **support_entitlement_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **user_id** | **String** |  | [optional] |
| **refund_policy_id** | **String** |  | [optional] |
| **payment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RefundRequestDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  approved: null,
  approved_timestamp: null,
  tenant_id: null,
  enrollment_id: null,
  support_entitlement_id: null,
  contact_id: null,
  user_id: null,
  refund_policy_id: null,
  payment_id: null
)
```

