# OpenapiClient::JournalEntryDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **group** | **Boolean** |  | [optional] |
| **opening** | **Boolean** |  | [optional] |
| **description** | **String** |  | [optional] |
| **date** | **Time** |  | [optional] |
| **forex_rates_snapshot** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **credit** | **Float** |  | [optional] |
| **debit** | **Float** |  | [optional] |
| **credit_in_usd** | **Float** |  | [optional] |
| **debit_in_usd** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **journal_id** | **String** |  | [optional] |
| **journal_name** | **String** |  | [optional] |
| **journal_code** | **String** |  | [optional] |
| **credit_account_id** | **String** |  | [optional] |
| **credit_account_name** | **String** |  | [optional] |
| **debit_account_id** | **String** |  | [optional] |
| **debit_account_name** | **String** |  | [optional] |
| **invoice_code** | **String** |  | [optional] |
| **parent_journal_entry_id** | **String** |  | [optional] |
| **credit_amount** | [**Money**](Money.md) |  | [optional] |
| **debit_amount** | [**Money**](Money.md) |  | [optional] |
| **credit_amount_in_usd** | [**Money**](Money.md) |  | [optional] |
| **debit_amount_in_usd** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalEntryDto.new(
  id: null,
  timestamp: null,
  group: null,
  opening: null,
  description: null,
  date: null,
  forex_rates_snapshot: null,
  forex_rate: null,
  credit: null,
  debit: null,
  credit_in_usd: null,
  debit_in_usd: null,
  currency_id: null,
  tenant_id: null,
  enrollment_id: null,
  journal_id: null,
  journal_name: null,
  journal_code: null,
  credit_account_id: null,
  credit_account_name: null,
  debit_account_id: null,
  debit_account_name: null,
  invoice_code: null,
  parent_journal_entry_id: null,
  credit_amount: null,
  debit_amount: null,
  credit_amount_in_usd: null,
  debit_amount_in_usd: null
)
```

