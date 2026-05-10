# OpenapiClient::ShippingMethodUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **cost** | **Float** |  | [optional] |
| **taxable** | **Boolean** |  | [optional] |
| **tax_included** | **Boolean** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **shipping_class_calculation_type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ShippingMethodUpdateDto.new(
  name: null,
  description: null,
  cost: null,
  taxable: null,
  tax_included: null,
  currency_id: null,
  shipping_class_calculation_type: null
)
```

