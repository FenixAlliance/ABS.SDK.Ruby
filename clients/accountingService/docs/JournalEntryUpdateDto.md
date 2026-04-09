# OpenapiClient::JournalEntryUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **group** | **Boolean** |  | [optional] |
| **opening** | **Boolean** |  | [optional] |
| **description** | **String** |  |  |
| **date** | **Time** |  |  |
| **debit** | **Float** |  | [optional] |
| **credit** | **Float** |  | [optional] |
| **journal_id** | **String** |  |  |
| **currency_id** | **String** |  |  |
| **invoice_code** | **String** |  | [optional] |
| **debit_account_id** | **String** |  |  |
| **credit_account_id** | **String** |  |  |
| **parent_journal_entry_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalEntryUpdateDto.new(
  group: null,
  opening: null,
  description: null,
  date: null,
  debit: null,
  credit: null,
  journal_id: null,
  currency_id: null,
  invoice_code: null,
  debit_account_id: null,
  credit_account_id: null,
  parent_journal_entry_id: null
)
```

