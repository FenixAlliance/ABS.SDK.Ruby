# OpenapiClient::ProofOfDeliveryLineDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **proof_of_delivery_id** | **String** |  | [optional] |
| **line_number** | **Integer** |  | [optional] |
| **description** | **String** |  | [optional] |
| **quantity_expected** | **Integer** |  | [optional] |
| **quantity_received** | **Integer** |  | [optional] |
| **quantity_rejected** | **Integer** |  | [optional] |
| **condition** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **hs_code** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ProofOfDeliveryLineDto.new(
  id: null,
  timestamp: null,
  proof_of_delivery_id: null,
  line_number: null,
  description: null,
  quantity_expected: null,
  quantity_received: null,
  quantity_rejected: null,
  condition: null,
  remarks: null,
  hs_code: null,
  tenant_id: null
)
```

