# OpenapiClient::ShippingLabelUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tracking_code** | **String** |  | [optional] |
| **expected_delivery** | **Time** |  | [optional] |
| **location_id** | **String** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |
| **shipping_courier_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ShippingLabelUpdateDto.new(
  tracking_code: null,
  expected_delivery: null,
  location_id: null,
  shipment_id: null,
  shipping_courier_id: null
)
```

