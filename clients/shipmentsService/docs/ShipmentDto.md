# OpenapiClient::ShipmentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **tracking_code** | **String** |  | [optional] |
| **is_international** | **Boolean** |  | [optional] |
| **shipment_timestamp** | **Time** |  | [optional] |
| **delivery_timestamp** | **Time** |  | [optional] |
| **expected_shipping_date** | **Time** |  | [optional] |
| **expected_delivery_date** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ShipmentDto.new(
  id: null,
  tracking_code: null,
  is_international: null,
  shipment_timestamp: null,
  delivery_timestamp: null,
  expected_shipping_date: null,
  expected_delivery_date: null
)
```

