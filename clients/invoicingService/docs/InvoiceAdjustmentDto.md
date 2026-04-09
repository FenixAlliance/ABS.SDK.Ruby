# OpenapiClient::InvoiceAdjustmentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
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

instance = OpenapiClient::InvoiceAdjustmentDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  invoice_id: null,
  currency_id: null,
  enrollment_id: null,
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

