# OpenapiClient::AccountingEntryUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **journal_entry_id** | **String** |  | [optional] |
| **account_id** | **String** |  | [optional] |
| **direction** | **String** |  | [optional] |
| **transaction_amount** | **Float** |  | [optional] |
| **transaction_currency_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AccountingEntryUpdateDto.new(
  journal_entry_id: null,
  account_id: null,
  direction: null,
  transaction_amount: null,
  transaction_currency_id: null,
  description: null
)
```

