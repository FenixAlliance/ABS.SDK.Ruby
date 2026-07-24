# OpenapiClient::AccountingEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **journal_entry_id** | **String** |  |  |
| **account_id** | **String** |  |  |
| **direction** | **String** |  |  |
| **transaction_amount** | **Float** |  | [optional] |
| **transaction_currency_id** | **String** |  |  |
| **description** | **String** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountingEntryCreateDto.new(
  id: null,
  timestamp: null,
  journal_entry_id: null,
  account_id: null,
  direction: null,
  transaction_amount: null,
  transaction_currency_id: null,
  description: null
)
```

