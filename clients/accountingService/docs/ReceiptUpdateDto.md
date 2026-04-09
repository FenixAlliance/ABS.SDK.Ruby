# OpenapiClient::ReceiptUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **payment_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **total_amount** | **Float** |  | [optional] |
| **total_amount_in_usd** | **Float** |  | [optional] |
| **closed** | **Boolean** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **account_holder_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ReceiptUpdateDto.new(
  payment_id: null,
  tenant_id: null,
  forex_rate: null,
  total_amount: null,
  total_amount_in_usd: null,
  closed: null,
  currency_id: null,
  account_holder_id: null,
  contact_id: null,
  enrollment_id: null,
  order_id: null,
  invoice_id: null
)
```

