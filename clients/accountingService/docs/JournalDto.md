# OpenapiClient::JournalDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **ledger_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **fiscal_year_id** | **String** |  | [optional] |
| **journal_type_id** | **String** |  | [optional] |
| **parent_journal_id** | **String** |  | [optional] |
| **financial_book_id** | **String** |  | [optional] |
| **code** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalDto.new(
  id: null,
  timestamp: null,
  name: null,
  description: null,
  tenant_id: null,
  ledger_id: null,
  enrollment_id: null,
  fiscal_year_id: null,
  journal_type_id: null,
  parent_journal_id: null,
  financial_book_id: null,
  code: null
)
```

