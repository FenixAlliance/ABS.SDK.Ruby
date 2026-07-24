# OpenapiClient::BudgetAccountEntryDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **planned_amount** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **debit_account_id** | **String** |  | [optional] |
| **credit_account_id** | **String** |  | [optional] |
| **budget_id** | **String** |  | [optional] |
| **date** | **Time** |  | [optional] |
| **planned_amount_money** | [**Money**](Money.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BudgetAccountEntryDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  enrollment_id: null,
  description: null,
  planned_amount: null,
  currency_id: null,
  debit_account_id: null,
  credit_account_id: null,
  budget_id: null,
  date: null,
  planned_amount_money: null
)
```

