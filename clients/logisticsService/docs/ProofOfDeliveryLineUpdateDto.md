# OpenapiClient::ProofOfDeliveryLineUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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

instance = OpenapiClient::ProofOfDeliveryLineUpdateDto.new(
  description: null,
  quantity_expected: null,
  quantity_received: null,
  quantity_rejected: null,
  condition: null,
  remarks: null,
  hs_code: null
)
```

