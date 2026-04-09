# OpenapiClient::InvoiceLineAppliedTaxDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **invoice_line_id** | **String** |  | [optional] |
| **tax_policy_id** | **String** |  | [optional] |
| **item_price_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **tax_amount_in_usd** | **Float** |  | [optional] |
| **tax_base_amount_in_usd** | **Float** |  | [optional] |
| **tax_policy_name** | **String** |  | [optional] |
| **tax_policy_description** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InvoiceLineAppliedTaxDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  invoice_id: null,
  enrollment_id: null,
  invoice_line_id: null,
  tax_policy_id: null,
  item_price_id: null,
  item_id: null,
  tax_amount_in_usd: null,
  tax_base_amount_in_usd: null,
  tax_policy_name: null,
  tax_policy_description: null
)
```

