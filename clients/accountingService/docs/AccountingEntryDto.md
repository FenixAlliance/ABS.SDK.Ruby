# OpenapiClient::AccountingEntryDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **debit** | **Float** |  | [optional] |
| **credit** | **Float** |  | [optional] |
| **description** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **account_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **date** | **Time** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **debit_account_id** | **String** |  | [optional] |
| **credit_account_id** | **String** |  | [optional] |
| **journal_entry_id** | **String** |  | [optional] |
| **debit_account_name** | **String** |  | [optional] |
| **credit_account_name** | **String** |  | [optional] |
| **accounting_entry_type** | **String** |  | [optional] |
| **debit_amount** | [**Money**](Money.md) |  | [optional] |
| **credit_amount** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountingEntryDto.new(
  id: null,
  timestamp: null,
  debit: null,
  credit: null,
  description: null,
  forex_rate: null,
  account_id: null,
  tenant_id: null,
  date: null,
  enrollment_id: null,
  currency_id: null,
  debit_account_id: null,
  credit_account_id: null,
  journal_entry_id: null,
  debit_account_name: null,
  credit_account_name: null,
  accounting_entry_type: null,
  debit_amount: null,
  credit_amount: null
)
```

