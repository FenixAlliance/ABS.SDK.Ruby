# OpenapiClient::ItemPriceCalculationEnvelope

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **is_success** | **Boolean** |  | [optional][readonly] |
| **error_message** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional][readonly] |
| **activity_id** | **String** |  | [optional][readonly] |
| **result** | [**ItemPriceCalculation**](ItemPriceCalculation.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ItemPriceCalculationEnvelope.new(
  is_success: null,
  error_message: null,
  correlation_id: null,
  timestamp: null,
  activity_id: null,
  result: null
)
```

