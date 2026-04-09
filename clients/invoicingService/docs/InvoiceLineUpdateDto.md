# OpenapiClient::InvoiceLineUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **price** | **Float** |  | [optional] |
| **unit_id** | **String** |  | [optional] |
| **percent** | **Float** |  | [optional] |
| **unit_group_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **discount_list_id** | **String** |  | [optional] |
| **rounding_policy_id** | **String** |  | [optional] |
| **quantity** | **Integer** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **item_price_id** | **String** |  | [optional] |
| **invoice_line_id** | **String** |  | [optional] |
| **tax_amount_in_usd** | **Float** |  | [optional] |
| **tax_base_amount_in_usd** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InvoiceLineUpdateDto.new(
  price: null,
  unit_id: null,
  percent: null,
  unit_group_id: null,
  currency_id: null,
  discount_list_id: null,
  rounding_policy_id: null,
  quantity: null,
  item_id: null,
  item_price_id: null,
  invoice_line_id: null,
  tax_amount_in_usd: null,
  tax_base_amount_in_usd: null
)
```

