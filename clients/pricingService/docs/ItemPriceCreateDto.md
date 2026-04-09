# OpenapiClient::ItemPriceCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **item_id** | **String** |  |  |
| **unit_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **price_list_id** | **String** |  | [optional] |
| **unit_group_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **discount_list_id** | **String** |  | [optional] |
| **rounding_policy_id** | **String** |  | [optional] |
| **price** | **Float** |  | [optional] |
| **percent** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ItemPriceCreateDto.new(
  id: null,
  timestamp: null,
  item_id: null,
  unit_id: null,
  tenant_id: null,
  currency_id: null,
  price_list_id: null,
  unit_group_id: null,
  enrollment_id: null,
  discount_list_id: null,
  rounding_policy_id: null,
  price: null,
  percent: null
)
```

