# OpenapiClient::ProofOfDeliveryDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **document_number** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
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
| **signed_by** | **String** |  | [optional] |
| **signer_identification** | **String** |  | [optional] |
| **signature_date** | **Time** |  | [optional] |
| **digital_signature_reference** | **String** |  | [optional] |
| **overall_condition** | **String** |  | [optional] |
| **total_quantity_delivered** | **Integer** |  | [optional] |
| **total_quantity_rejected** | **Integer** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **photo_evidence_uri** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **lines** | [**Array&lt;ProofOfDeliveryLineDto&gt;**](ProofOfDeliveryLineDto.md) |  | [optional] |
| **delivery_note_ids** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ProofOfDeliveryDto.new(
  id: null,
  timestamp: null,
  document_number: null,
  status: null,
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
  signed_by: null,
  signer_identification: null,
  signature_date: null,
  digital_signature_reference: null,
  overall_condition: null,
  total_quantity_delivered: null,
  total_quantity_rejected: null,
  remarks: null,
  photo_evidence_uri: null,
  tenant_id: null,
  enrollment_id: null,
  lines: null,
  delivery_note_ids: null
)
```

