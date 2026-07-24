# OpenapiClient::JournalEntryUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **fiscal_period_id** | **String** |  |  |
| **transaction_currency_id** | **String** |  |  |
| **description** | **String** |  |  |
| **source_document_type** | **String** |  | [optional] |
| **source_document_id** | **String** |  | [optional] |
| **is_opening_balance** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalEntryUpdateDto.new(
  fiscal_period_id: null,
  transaction_currency_id: null,
  description: null,
  source_document_type: null,
  source_document_id: null,
  is_opening_balance: null
)
```

