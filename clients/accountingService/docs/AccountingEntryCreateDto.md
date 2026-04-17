# OpenapiClient::AccountingEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **description** | **String** |  |  |
| **date** | **Time** |  | [optional] |
| **amount** | **Float** |  | [optional] |
| **currency_id** | **String** |  |  |
| **debit_account_id** | **String** |  | [optional] |
| **credit_account_id** | **String** |  | [optional] |
| **journal_entry_id** | **String** |  | [optional] |
| **accounting_entry_type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountingEntryCreateDto.new(
  id: null,
  timestamp: null,
  description: null,
  date: null,
  amount: null,
  currency_id: null,
  debit_account_id: null,
  credit_account_id: null,
  journal_entry_id: null,
  accounting_entry_type: null
)
```

