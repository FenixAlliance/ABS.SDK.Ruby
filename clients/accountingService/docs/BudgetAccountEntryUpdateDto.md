# OpenapiClient::BudgetAccountEntryUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **amount** | **Float** |  | [optional] |
| **date** | **Time** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **debit_account_id** | **String** |  | [optional] |
| **credit_account_id** | **String** |  | [optional] |
| **journal_entry_id** | **String** |  | [optional] |
| **accounting_entry_type** | **String** |  | [optional] |
| **budget_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BudgetAccountEntryUpdateDto.new(
  tenant_id: null,
  enrollment_id: null,
  description: null,
  amount: null,
  date: null,
  currency_id: null,
  debit_account_id: null,
  credit_account_id: null,
  journal_entry_id: null,
  accounting_entry_type: null,
  budget_id: null
)
```

