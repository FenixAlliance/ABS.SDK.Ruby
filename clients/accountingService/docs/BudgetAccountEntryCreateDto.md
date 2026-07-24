# OpenapiClient::BudgetAccountEntryCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **description** | **String** |  |  |
| **planned_amount** | **Float** |  | [optional] |
| **currency_id** | **String** |  |  |
| **debit_account_id** | **String** |  |  |
| **credit_account_id** | **String** |  |  |
| **budget_id** | **String** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BudgetAccountEntryCreateDto.new(
  id: null,
  timestamp: null,
  description: null,
  planned_amount: null,
  currency_id: null,
  debit_account_id: null,
  credit_account_id: null,
  budget_id: null
)
```

