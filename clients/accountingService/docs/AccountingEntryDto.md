# OpenapiClient::AccountingEntryDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **journal_entry_id** | **String** |  | [optional] |
| **account_id** | **String** |  | [optional] |
| **account_name** | **String** |  | [optional] |
| **direction** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **transaction_amount** | **Float** |  | [optional] |
| **transaction_currency_id** | **String** |  | [optional] |
| **functional_amount** | **Float** |  | [optional] |
| **functional_currency_id** | **String** |  | [optional] |
| **account_amount** | **Float** |  | [optional] |
| **account_currency_id** | **String** |  | [optional] |
| **reporting_amount_in_usd** | **Float** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **forex_rates_snapshot** | **String** |  | [optional] |
| **cost_centre_id** | **String** |  | [optional] |
| **project_id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **debit** | **Float** |  | [optional][readonly] |
| **credit** | **Float** |  | [optional][readonly] |
| **amount** | [**Money**](Money.md) |  | [optional] |
| **amount_in_usd** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountingEntryDto.new(
  id: null,
  tenant_id: null,
  enrollment_id: null,
  journal_entry_id: null,
  account_id: null,
  account_name: null,
  direction: null,
  description: null,
  transaction_amount: null,
  transaction_currency_id: null,
  functional_amount: null,
  functional_currency_id: null,
  account_amount: null,
  account_currency_id: null,
  reporting_amount_in_usd: null,
  forex_rate: null,
  forex_rates_snapshot: null,
  cost_centre_id: null,
  project_id: null,
  timestamp: null,
  debit: null,
  credit: null,
  amount: null,
  amount_in_usd: null
)
```

