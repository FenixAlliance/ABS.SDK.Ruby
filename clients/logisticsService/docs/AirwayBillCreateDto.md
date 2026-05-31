# OpenapiClient::AirwayBillCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **document_number** | **String** |  | [optional] |
| **airway_bill_type** | **String** |  | [optional] |
| **master_awb_number** | **String** |  | [optional] |
| **shipper_contact_id** | **String** |  | [optional] |
| **consignee_contact_id** | **String** |  | [optional] |
| **notify_party_contact_id** | **String** |  | [optional] |
| **carrier_id** | **String** |  | [optional] |
| **airline_code** | **String** |  | [optional] |
| **flight_number** | **String** |  | [optional] |
| **airport_of_departure_code** | **String** |  | [optional] |
| **airport_of_destination_code** | **String** |  | [optional] |
| **departure_date** | **Time** |  | [optional] |
| **arrival_date** | **Time** |  | [optional] |
| **date_issued** | **Time** |  | [optional] |
| **freight_terms** | **String** |  | [optional] |
| **freight_amount** | **Float** |  | [optional] |
| **freight_currency_id** | **String** |  | [optional] |
| **chargeable_weight_kg** | **Float** |  | [optional] |
| **total_gross_weight_kg** | **Float** |  | [optional] |
| **total_packages** | **Integer** |  | [optional] |
| **total_volume_m3** | **Float** |  | [optional] |
| **declared_value_for_carriage** | **Float** |  | [optional] |
| **declared_value_for_customs** | **Float** |  | [optional] |
| **insurance_amount** | **Float** |  | [optional] |
| **special_handling_codes** | **String** |  | [optional] |
| **special_instructions** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AirwayBillCreateDto.new(
  id: null,
  timestamp: null,
  document_number: null,
  airway_bill_type: null,
  master_awb_number: null,
  shipper_contact_id: null,
  consignee_contact_id: null,
  notify_party_contact_id: null,
  carrier_id: null,
  airline_code: null,
  flight_number: null,
  airport_of_departure_code: null,
  airport_of_destination_code: null,
  departure_date: null,
  arrival_date: null,
  date_issued: null,
  freight_terms: null,
  freight_amount: null,
  freight_currency_id: null,
  chargeable_weight_kg: null,
  total_gross_weight_kg: null,
  total_packages: null,
  total_volume_m3: null,
  declared_value_for_carriage: null,
  declared_value_for_customs: null,
  insurance_amount: null,
  special_handling_codes: null,
  special_instructions: null,
  remarks: null,
  shipment_id: null
)
```

