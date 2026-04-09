# OpenapiClient::AppliedTaxPolicyRecordUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **tax_policy_id** | **String** |  | [optional] |
| **invoice_id** | **String** |  | [optional] |
| **item_id** | **String** |  | [optional] |
| **tax_amount_in_usd** | **Float** |  | [optional] |
| **tax_base_amount_in_usd** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AppliedTaxPolicyRecordUpdateDto.new(
  tenant_id: null,
  enrollment_id: null,
  tax_policy_id: null,
  invoice_id: null,
  item_id: null,
  tax_amount_in_usd: null,
  tax_base_amount_in_usd: null
)
```

