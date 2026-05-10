# OpenapiClient::ItemRestockEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **item_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **item_restock_id** | **String** |  |  |
| **quantity** | **Float** |  | [optional] |
| **order_item_record_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ItemRestockEntryCreateDto.new(
  id: null,
  timestamp: null,
  item_id: null,
  warehouse_id: null,
  item_restock_id: null,
  quantity: null,
  order_item_record_id: null
)
```

