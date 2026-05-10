# OpenapiClient::ShipmentCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tracking_code** | **String** |  | [optional] |
| **is_international** | **Boolean** |  | [optional] |
| **expected_shipping_date** | **Time** |  | [optional] |
| **expected_delivery_date** | **Time** |  | [optional] |
| **shipping_terms** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ShipmentCreateDto.new(
  id: null,
  timestamp: null,
  tracking_code: null,
  is_international: null,
  expected_shipping_date: null,
  expected_delivery_date: null,
  shipping_terms: null,
  order_id: null
)
```

