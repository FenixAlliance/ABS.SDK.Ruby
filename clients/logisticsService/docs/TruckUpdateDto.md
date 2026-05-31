# OpenapiClient::TruckUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **plate_number** | **String** |  | [optional] |
| **name** | **String** |  | [optional] |
| **truck_type** | **String** |  | [optional] |
| **max_payload_kg** | **Float** |  | [optional] |
| **teu_capacity** | **Integer** |  | [optional] |
| **driver_name** | **String** |  | [optional] |
| **driver_phone** | **String** |  | [optional] |
| **driver_license_number** | **String** |  | [optional] |
| **is_active** | **Boolean** |  | [optional] |
| **is_refrigerated** | **Boolean** |  | [optional] |
| **shipping_courier_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TruckUpdateDto.new(
  plate_number: null,
  name: null,
  truck_type: null,
  max_payload_kg: null,
  teu_capacity: null,
  driver_name: null,
  driver_phone: null,
  driver_license_number: null,
  is_active: null,
  is_refrigerated: null,
  shipping_courier_id: null
)
```

