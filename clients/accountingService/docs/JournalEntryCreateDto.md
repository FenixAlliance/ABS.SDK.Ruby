# OpenapiClient::JournalEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **journal_id** | **String** |  |  |
| **fiscal_period_id** | **String** |  |  |
| **transaction_currency_id** | **String** |  |  |
| **description** | **String** |  |  |
| **source_document_type** | **String** |  | [optional] |
| **source_document_id** | **String** |  | [optional] |
| **idempotency_key** | **String** |  | [optional] |
| **is_opening_balance** | **Boolean** |  | [optional] |
| **accounting_entries** | [**Array&lt;AccountingEntryCreateDto&gt;**](AccountingEntryCreateDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JournalEntryCreateDto.new(
  id: null,
  timestamp: null,
  journal_id: null,
  fiscal_period_id: null,
  transaction_currency_id: null,
  description: null,
  source_document_type: null,
  source_document_id: null,
  idempotency_key: null,
  is_opening_balance: null,
  accounting_entries: null
)
```

