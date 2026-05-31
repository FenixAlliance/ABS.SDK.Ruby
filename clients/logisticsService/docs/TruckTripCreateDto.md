# OpenapiClient::TruckTripCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **trip_number** | **String** |  | [optional] |
| **container_number** | **String** |  | [optional] |
| **seal_number** | **String** |  | [optional] |
| **departure_time** | **Time** |  | [optional] |
| **arrival_time** | **Time** |  | [optional] |
| **distance_km** | **Float** |  | [optional] |
| **notes** | **String** |  | [optional] |
| **origin_port_id** | **String** |  | [optional] |
| **origin_location_id** | **String** |  | [optional] |
| **destination_port_id** | **String** |  | [optional] |
| **destination_location_id** | **String** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |
| **bill_of_lading_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TruckTripCreateDto.new(
  id: null,
  timestamp: null,
  trip_number: null,
  container_number: null,
  seal_number: null,
  departure_time: null,
  arrival_time: null,
  distance_km: null,
  notes: null,
  origin_port_id: null,
  origin_location_id: null,
  destination_port_id: null,
  destination_location_id: null,
  shipment_id: null,
  bill_of_lading_id: null
)
```

