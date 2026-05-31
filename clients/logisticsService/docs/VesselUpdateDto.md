# OpenapiClient::VesselUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **imo_number** | **String** |  | [optional] |
| **mmsi_number** | **String** |  | [optional] |
| **call_sign** | **String** |  | [optional] |
| **flag_country_id** | **String** |  | [optional] |
| **vessel_type** | **String** |  | [optional] |
| **vessel_status** | **String** |  | [optional] |
| **gross_tonnage** | **Float** |  | [optional] |
| **deadweight_tonnage** | **Float** |  | [optional] |
| **teu_capacity** | **Integer** |  | [optional] |
| **length_meters** | **Float** |  | [optional] |
| **beam_meters** | **Float** |  | [optional] |
| **draft_meters** | **Float** |  | [optional] |
| **year_built** | **Integer** |  | [optional] |
| **shipping_courier_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::VesselUpdateDto.new(
  name: null,
  imo_number: null,
  mmsi_number: null,
  call_sign: null,
  flag_country_id: null,
  vessel_type: null,
  vessel_status: null,
  gross_tonnage: null,
  deadweight_tonnage: null,
  teu_capacity: null,
  length_meters: null,
  beam_meters: null,
  draft_meters: null,
  year_built: null,
  shipping_courier_id: null
)
```

