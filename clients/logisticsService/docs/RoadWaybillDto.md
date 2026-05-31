# OpenapiClient::RoadWaybillDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **document_number** | **String** |  | [optional] |
| **road_waybill_type** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **shipper_contact_id** | **String** |  | [optional] |
| **consignee_contact_id** | **String** |  | [optional] |
| **carrier_id** | **String** |  | [optional] |
| **successive_carriers** | **String** |  | [optional] |
| **truck_id** | **String** |  | [optional] |
| **truck_driver_id** | **String** |  | [optional] |
| **vehicle_registration** | **String** |  | [optional] |
| **trailer_registration** | **String** |  | [optional] |
| **place_of_taking_over** | **String** |  | [optional] |
| **place_of_taking_over_port_id** | **String** |  | [optional] |
| **place_of_delivery** | **String** |  | [optional] |
| **place_of_delivery_port_id** | **String** |  | [optional] |
| **date_of_taking_over** | **Time** |  | [optional] |
| **date_of_delivery** | **Time** |  | [optional] |
| **freight_terms** | **String** |  | [optional] |
| **freight_amount** | **Float** |  | [optional] |
| **freight_currency_id** | **String** |  | [optional] |
| **total_gross_weight_kg** | **Float** |  | [optional] |
| **total_packages** | **Integer** |  | [optional] |
| **total_volume_m3** | **Float** |  | [optional] |
| **adr_dangerous_goods** | **Boolean** |  | [optional] |
| **special_instructions** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **sender_signed_date** | **Time** |  | [optional] |
| **carrier_signed_date** | **Time** |  | [optional] |
| **consignee_signed_date** | **Time** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |
| **truck_trip_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **lines** | [**Array&lt;WaybillLineDto&gt;**](WaybillLineDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RoadWaybillDto.new(
  id: null,
  timestamp: null,
  document_number: null,
  road_waybill_type: null,
  status: null,
  shipper_contact_id: null,
  consignee_contact_id: null,
  carrier_id: null,
  successive_carriers: null,
  truck_id: null,
  truck_driver_id: null,
  vehicle_registration: null,
  trailer_registration: null,
  place_of_taking_over: null,
  place_of_taking_over_port_id: null,
  place_of_delivery: null,
  place_of_delivery_port_id: null,
  date_of_taking_over: null,
  date_of_delivery: null,
  freight_terms: null,
  freight_amount: null,
  freight_currency_id: null,
  total_gross_weight_kg: null,
  total_packages: null,
  total_volume_m3: null,
  adr_dangerous_goods: null,
  special_instructions: null,
  remarks: null,
  sender_signed_date: null,
  carrier_signed_date: null,
  consignee_signed_date: null,
  shipment_id: null,
  truck_trip_id: null,
  tenant_id: null,
  enrollment_id: null,
  lines: null
)
```

