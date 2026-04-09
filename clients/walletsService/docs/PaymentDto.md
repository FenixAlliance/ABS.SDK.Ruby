# OpenapiClient::PaymentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **test** | **Boolean** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **emisor_wallet_id** | **String** |  | [optional] |
| **receiver_wallet_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **total_cost** | **Float** |  | [optional] |
| **total_taxes** | **Float** |  | [optional] |
| **closed** | **Boolean** |  | [optional] |
| **data** | **String** |  | [optional] |
| **data_label** | **String** |  | [optional] |
| **data1** | **String** |  | [optional] |
| **data1_label** | **String** |  | [optional] |
| **response** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |
| **reference_code** | **String** |  | [optional] |
| **correlation_code** | **String** |  | [optional] |
| **last_updated** | **Time** |  | [optional] |
| **on_behalf_of** | **String** |  | [optional] |
| **payment_type** | **String** |  | [optional] |
| **payment_status** | **String** |  | [optional] |
| **base_cost** | **Float** |  | [optional] |
| **signature** | **String** |  | [optional] |
| **signature_mismatch** | **Boolean** |  | [optional] |
| **is_external** | **Boolean** |  | [optional] |
| **marked_for_revision** | **Boolean** |  | [optional] |
| **forex_rates_snapshot** | **String** |  | [optional] |
| **official_id** | **String** |  | [optional] |
| **official_id_expedition_date** | **Time** |  | [optional] |
| **fiscal_identification_type_id** | **String** |  | [optional] |
| **billing_address** | **String** |  | [optional] |
| **phone** | **String** |  | [optional] |
| **cellphone** | **String** |  | [optional] |
| **department** | **String** |  | [optional] |
| **city** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **location_id** | **String** |  | [optional] |
| **entitlement_id** | **String** |  | [optional] |
| **anti_fraud_score** | **Float** |  | [optional] |
| **call_record_url** | **String** |  | [optional] |
| **called** | **Boolean** |  | [optional] |
| **verified** | **Boolean** |  | [optional] |
| **payer_picture_timestamp** | **String** |  | [optional] |
| **payer_picture** | **String** |  | [optional] |
| **identification_picture_timestamp** | **String** |  | [optional] |
| **identification_picture** | **String** |  | [optional] |
| **identification_back_picture** | **String** |  | [optional] |
| **identification_back_picture_timestamp** | **String** |  | [optional] |
| **ip_lookup_id** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |
| **accounting_entry_id** | **String** |  | [optional] |
| **payment_gateway_id** | **String** |  | [optional] |
| **bank_account_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **bank_id** | **String** |  | [optional] |
| **payment_token_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentDto.new(
  id: null,
  timestamp: null,
  test: null,
  invoice_id: null,
  tenant_id: null,
  emisor_wallet_id: null,
  receiver_wallet_id: null,
  currency_id: null,
  forex_rate: null,
  total_cost: null,
  total_taxes: null,
  closed: null,
  data: null,
  data_label: null,
  data1: null,
  data1_label: null,
  response: null,
  authorization: null,
  reference_code: null,
  correlation_code: null,
  last_updated: null,
  on_behalf_of: null,
  payment_type: null,
  payment_status: null,
  base_cost: null,
  signature: null,
  signature_mismatch: null,
  is_external: null,
  marked_for_revision: null,
  forex_rates_snapshot: null,
  official_id: null,
  official_id_expedition_date: null,
  fiscal_identification_type_id: null,
  billing_address: null,
  phone: null,
  cellphone: null,
  department: null,
  city: null,
  country_id: null,
  location_id: null,
  entitlement_id: null,
  anti_fraud_score: null,
  call_record_url: null,
  called: null,
  verified: null,
  payer_picture_timestamp: null,
  payer_picture: null,
  identification_picture_timestamp: null,
  identification_picture: null,
  identification_back_picture: null,
  identification_back_picture_timestamp: null,
  ip_lookup_id: null,
  order_id: null,
  accounting_entry_id: null,
  payment_gateway_id: null,
  bank_account_id: null,
  enrollment_id: null,
  bank_id: null,
  payment_token_id: null
)
```

