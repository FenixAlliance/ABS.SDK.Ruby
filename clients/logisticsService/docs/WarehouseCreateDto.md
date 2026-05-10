# OpenapiClient::WarehouseCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **address1** | **String** |  |  |
| **address2** | **String** |  | [optional] |
| **address3** | **String** |  | [optional] |
| **postal_code** | **String** |  | [optional] |
| **phone** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **state_id** | **String** |  | [optional] |
| **city_id** | **String** |  | [optional] |
| **is_group** | **Boolean** |  | [optional] |
| **shipwire_warehouse_id** | **String** |  | [optional] |
| **parent_warehouse_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WarehouseCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  address1: null,
  address2: null,
  address3: null,
  postal_code: null,
  phone: null,
  country_id: null,
  state_id: null,
  city_id: null,
  is_group: null,
  shipwire_warehouse_id: null,
  parent_warehouse_id: null
)
```

