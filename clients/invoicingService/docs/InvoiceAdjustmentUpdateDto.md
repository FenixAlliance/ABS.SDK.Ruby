# OpenapiClient::InvoiceAdjustmentUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **currency_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **surcharge_percent** | **Float** |  | [optional] |
| **surcharge_amount** | **Float** |  | [optional] |
| **discount_percent** | **Float** |  | [optional] |
| **discount_amount** | **Float** |  | [optional] |
| **total_surcharge** | **Float** |  | [optional] |
| **total_discount** | **Float** |  | [optional] |
| **type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InvoiceAdjustmentUpdateDto.new(
  currency_id: null,
  description: null,
  surcharge_percent: null,
  surcharge_amount: null,
  discount_percent: null,
  discount_amount: null,
  total_surcharge: null,
  total_discount: null,
  type: null
)
```

