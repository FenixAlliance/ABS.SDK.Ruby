# OpenapiClient::ProofOfDeliveryLineCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **description** | **String** |  | [optional] |
| **quantity_expected** | **Integer** |  | [optional] |
| **quantity_received** | **Integer** |  | [optional] |
| **quantity_rejected** | **Integer** |  | [optional] |
| **condition** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **hs_code** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ProofOfDeliveryLineCreateDto.new(
  id: null,
  timestamp: null,
  description: null,
  quantity_expected: null,
  quantity_received: null,
  quantity_rejected: null,
  condition: null,
  remarks: null,
  hs_code: null
)
```

