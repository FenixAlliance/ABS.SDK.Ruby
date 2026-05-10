# OpenapiClient::AppliedItemTaxRecordUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tax_policy_id** | **String** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **tax_amount_in_usd** | **Float** |  | [optional] |
| **tax_base_amount_in_usd** | **Float** |  | [optional] |
| **billing_item_record_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AppliedItemTaxRecordUpdateDto.new(
  tax_policy_id: null,
  invoice_id: null,
  item_id: null,
  tax_amount_in_usd: null,
  tax_base_amount_in_usd: null,
  billing_item_record_id: null
)
```

