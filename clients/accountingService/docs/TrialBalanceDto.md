# OpenapiClient::TrialBalanceDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **fiscal_period_id** | **String** |  | [optional] |
| **financial_book_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **rows** | [**Array&lt;TrialBalanceRowDto&gt;**](TrialBalanceRowDto.md) |  | [optional] |
| **total_debit** | **Float** |  | [optional] |
| **total_credit** | **Float** |  | [optional] |
| **is_balanced** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TrialBalanceDto.new(
  fiscal_period_id: null,
  financial_book_id: null,
  currency_id: null,
  rows: null,
  total_debit: null,
  total_credit: null,
  is_balanced: null
)
```

