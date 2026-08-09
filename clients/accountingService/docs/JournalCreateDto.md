# OpenapiClient::JournalCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **date_time** | **Time** |  | [optional] |
| **parent_journal_id** | **String** |  | [optional] |
| **journal_type_id** | **String** |  | [optional] |
| **ledger_id** | **String** |  | [optional] |
| **financial_book_id** | **String** |  | [optional] |
| **code** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalCreateDto.new(
  id: null,
  timestamp: null,
  name: null,
  description: null,
  date_time: null,
  parent_journal_id: null,
  journal_type_id: null,
  ledger_id: null,
  financial_book_id: null,
  code: null
)
```

