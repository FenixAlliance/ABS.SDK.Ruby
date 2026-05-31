# OpenapiClient::SeawayBillDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **document_number** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **shipper_contact_id** | **String** |  | [optional] |
| **consignee_contact_id** | **String** |  | [optional] |
| **notify_party_contact_id** | **String** |  | [optional] |
| **carrier_id** | **String** |  | [optional] |
| **vessel_id** | **String** |  | [optional] |
| **voyage_id** | **String** |  | [optional] |
| **port_of_loading_id** | **String** |  | [optional] |
| **port_of_discharge_id** | **String** |  | [optional] |
| **place_of_receipt** | **String** |  | [optional] |
| **place_of_delivery** | **String** |  | [optional] |
| **date_issued** | **Time** |  | [optional] |
| **date_shipped** | **Time** |  | [optional] |
| **date_delivered** | **Time** |  | [optional] |
| **freight_terms** | **String** |  | [optional] |
| **freight_amount** | **Float** |  | [optional] |
| **freight_currency_id** | **String** |  | [optional] |
| **total_weight** | **Float** |  | [optional] |
| **total_packages** | **Integer** |  | [optional] |
| **special_instructions** | **String** |  | [optional] |
| **remarks** | **String** |  | [optional] |
| **shipment_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **lines** | [**Array&lt;WaybillLineDto&gt;**](WaybillLineDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SeawayBillDto.new(
  id: null,
  timestamp: null,
  document_number: null,
  status: null,
  shipper_contact_id: null,
  consignee_contact_id: null,
  notify_party_contact_id: null,
  carrier_id: null,
  vessel_id: null,
  voyage_id: null,
  port_of_loading_id: null,
  port_of_discharge_id: null,
  place_of_receipt: null,
  place_of_delivery: null,
  date_issued: null,
  date_shipped: null,
  date_delivered: null,
  freight_terms: null,
  freight_amount: null,
  freight_currency_id: null,
  total_weight: null,
  total_packages: null,
  special_instructions: null,
  remarks: null,
  shipment_id: null,
  tenant_id: null,
  enrollment_id: null,
  lines: null
)
```

