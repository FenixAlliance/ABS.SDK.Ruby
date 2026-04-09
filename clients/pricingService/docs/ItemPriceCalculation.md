# OpenapiClient::ItemPriceCalculation

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quantity** | **Float** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **item** | **String** |  | [optional] |
| **unit_id** | **String** |  | [optional] |
| **unit_group_id** | **String** |  | [optional] |
| **price_id** | **String** |  | [optional] |
| **price_list_id** | **String** |  | [optional] |
| **discount_id** | **String** |  | [optional] |
| **discount_list_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **rounding_policy_id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **effective_discount_percent** | **Float** |  | [optional][readonly] |
| **effective_tax_percent** | **Float** |  | [optional][readonly] |
| **currency_id** | **String** |  | [optional] |
| **currency** | [**CurrencyId**](CurrencyId.md) |  | [optional] |
| **total_base_amount** | [**Money**](Money.md) |  | [optional] |
| **total_profit_amount** | [**Money**](Money.md) |  | [optional] |
| **total_detail_amount** | [**Money**](Money.md) |  | [optional] |
| **total_discounts_amount** | [**Money**](Money.md) |  | [optional] |
| **total_surcharges_amount** | [**Money**](Money.md) |  | [optional] |
| **total_tax_base_amount** | [**Money**](Money.md) |  | [optional] |
| **total_tax_amount** | [**Money**](Money.md) |  | [optional] |
| **total_w_tax_amount** | [**Money**](Money.md) |  | [optional] |
| **total_shipping_cost_amount** | [**Money**](Money.md) |  | [optional] |
| **total_shipping_tax_amount** | [**Money**](Money.md) |  | [optional] |
| **total_amount** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ItemPriceCalculation.new(
  quantity: null,
  item_id: null,
  item: null,
  unit_id: null,
  unit_group_id: null,
  price_id: null,
  price_list_id: null,
  discount_id: null,
  discount_list_id: null,
  tenant_id: null,
  enrollment_id: null,
  rounding_policy_id: null,
  timestamp: null,
  effective_discount_percent: null,
  effective_tax_percent: null,
  currency_id: null,
  currency: null,
  total_base_amount: null,
  total_profit_amount: null,
  total_detail_amount: null,
  total_discounts_amount: null,
  total_surcharges_amount: null,
  total_tax_base_amount: null,
  total_tax_amount: null,
  total_w_tax_amount: null,
  total_shipping_cost_amount: null,
  total_shipping_tax_amount: null,
  total_amount: null
)
```

