# OpenapiClient::ShipmentUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tracking_code** | **String** |  | [optional] |
| **is_international** | **Boolean** |  | [optional] |
| **shipped** | **Boolean** |  | [optional] |
| **delivered** | **Boolean** |  | [optional] |
| **shipment_timestamp** | **Time** |  | [optional] |
| **delivery_timestamp** | **Time** |  | [optional] |
| **expected_shipping_date** | **Time** |  | [optional] |
| **expected_delivery_date** | **Time** |  | [optional] |
| **shipping_terms** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ShipmentUpdateDto.new(
  tracking_code: null,
  is_international: null,
  shipped: null,
  delivered: null,
  shipment_timestamp: null,
  delivery_timestamp: null,
  expected_shipping_date: null,
  expected_delivery_date: null,
  shipping_terms: null,
  order_id: null
)
```

