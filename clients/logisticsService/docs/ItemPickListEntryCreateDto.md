# OpenapiClient::ItemPickListEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **item_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **item_pick_list_id** | **String** |  |  |
| **quantity** | **Float** |  | [optional] |
| **order_item_record_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ItemPickListEntryCreateDto.new(
  id: null,
  timestamp: null,
  item_id: null,
  warehouse_id: null,
  item_pick_list_id: null,
  quantity: null,
  order_item_record_id: null
)
```

