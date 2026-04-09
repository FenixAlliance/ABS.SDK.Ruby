# OpenapiClient::JournalEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **group** | **Boolean** |  | [optional] |
| **opening** | **Boolean** |  | [optional] |
| **description** | **String** |  |  |
| **date** | **Time** |  |  |
| **debit** | **Float** |  | [optional] |
| **credit** | **Float** |  | [optional] |
| **journal_id** | **String** |  |  |
| **currency_id** | **String** |  |  |
| **debit_account_id** | **String** |  |  |
| **credit_account_id** | **String** |  |  |
| **parent_journal_entry_id** | **String** |  | [optional] |
| **invoice_code** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalEntryCreateDto.new(
  id: null,
  timestamp: null,
  group: null,
  opening: null,
  description: null,
  date: null,
  debit: null,
  credit: null,
  journal_id: null,
  currency_id: null,
  debit_account_id: null,
  credit_account_id: null,
  parent_journal_entry_id: null,
  invoice_code: null
)
```

