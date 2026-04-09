# OpenapiClient::AppliedTaxPolicyRecordDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
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

instance = OpenapiClient::AppliedTaxPolicyRecordDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  enrollment_id: null,
  tax_policy_id: null,
  invoice_id: null,
  item_id: null,
  tax_amount_in_usd: null,
  tax_base_amount_in_usd: null
)
```

