# OpenapiClient::TaxRateCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  | [optional] |
| **rate** | **Float** |  | [optional] |
| **value** | **Float** |  | [optional] |
| **um** | **String** |  | [optional] |
| **unit_id** | **String** |  | [optional] |
| **unit_group_id** | **String** |  | [optional] |
| **priority** | **Integer** |  | [optional] |
| **compound** | **Boolean** |  | [optional] |
| **shipping** | **Boolean** |  | [optional] |
| **withholding** | **Boolean** |  | [optional] |
| **single_transaction_threshold** | **Float** |  | [optional] |
| **cumulative_transaction_threshold** | **Float** |  | [optional] |
| **fiscal_authority_id** | **String** |  | [optional] |
| **fiscal_year_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **country_id** | **String** |  | [optional] |
| **tax_class_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **tax_policy_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TaxRateCreateDto.new(
  id: null,
  timestamp: null,
  name: null,
  rate: null,
  value: null,
  um: null,
  unit_id: null,
  unit_group_id: null,
  priority: null,
  compound: null,
  shipping: null,
  withholding: null,
  single_transaction_threshold: null,
  cumulative_transaction_threshold: null,
  fiscal_authority_id: null,
  fiscal_year_id: null,
  tenant_id: null,
  country_id: null,
  tax_class_id: null,
  currency_id: null,
  tax_policy_id: null,
  enrollment_id: null
)
```

