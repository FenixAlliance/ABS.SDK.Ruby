# OpenapiClient::RailWaybillUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **document_number** | **String** |  | [optional] |
| **shipper_contact_id** | **String** |  | [optional] |
| **consignee_contact_id** | **String** |  | [optional] |
| **carrier_id** | **String** |  | [optional] |
| **rail_operator_name** | **String** |  | [optional] |
| **station_of_departure** | **String** |  | [optional] |
| **station_of_departure_code** | **String** |  | [optional] |
| **station_of_destination** | **String** |  | [optional] |
| **station_of_destination_code** | **String** |  | [optional] |
| **prescribed_route** | **String** |  | [optional] |
| **wagon_numbers** | **String** |  | [optional] |
| **date_of_acceptance** | **Time** |  | [optional] |
| **date_of_delivery** | **Time** |  | [optional] |
| **freight_terms** | **String** |  | [optional] |
| **freight_amount** | **Float** |  | [optional] |
| **freight_currency_id** | **String** |  | [optional] |
| **total_gross_weight_kg** | **Float** |  | [optional] |
| **total_packages** | **Integer** |  | [optional] |
| **total_volume_m3** | **Float** |  | [optional] |
| **customs_formalities** | **String** |  | [optional] |
| **special_instructions** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RailWaybillUpdateDto.new(
  document_number: null,
  shipper_contact_id: null,
  consignee_contact_id: null,
  carrier_id: null,
  rail_operator_name: null,
  station_of_departure: null,
  station_of_departure_code: null,
  station_of_destination: null,
  station_of_destination_code: null,
  prescribed_route: null,
  wagon_numbers: null,
  date_of_acceptance: null,
  date_of_delivery: null,
  freight_terms: null,
  freight_amount: null,
  freight_currency_id: null,
  total_gross_weight_kg: null,
  total_packages: null,
  total_volume_m3: null,
  customs_formalities: null,
  special_instructions: null,
  remarks: null,
  shipment_id: null
)
```

