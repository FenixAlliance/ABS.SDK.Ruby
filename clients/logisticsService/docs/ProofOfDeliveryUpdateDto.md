# OpenapiClient::ProofOfDeliveryUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **document_number** | **String** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |
| **bill_of_lading_id** | **String** |  | [optional] |
| **seaway_bill_id** | **String** |  | [optional] |
| **airway_bill_id** | **String** |  | [optional] |
| **road_waybill_id** | **String** |  | [optional] |
| **rail_waybill_id** | **String** |  | [optional] |
| **truck_trip_id** | **String** |  | [optional] |
| **recipient_name** | **String** |  | [optional] |
| **recipient_company_contact_id** | **String** |  | [optional] |
| **delivery_address** | **String** |  | [optional] |
| **delivery_date** | **Time** |  | [optional] |
| **delivery_time** | **String** |  | [optional] |
| **overall_condition** | **String** |  | [optional] |
| **total_quantity_delivered** | **Integer** |  | [optional] |
| **total_quantity_rejected** | **Integer** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **photo_evidence_uri** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ProofOfDeliveryUpdateDto.new(
  document_number: null,
  shipment_id: null,
  bill_of_lading_id: null,
  seaway_bill_id: null,
  airway_bill_id: null,
  road_waybill_id: null,
  rail_waybill_id: null,
  truck_trip_id: null,
  recipient_name: null,
  recipient_company_contact_id: null,
  delivery_address: null,
  delivery_date: null,
  delivery_time: null,
  overall_condition: null,
  total_quantity_delivered: null,
  total_quantity_rejected: null,
  remarks: null,
  photo_evidence_uri: null
)
```

