# OpenapiClient::LoanCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **loan_timestamp** | **Time** |  | [optional] |
| **payment_deadline** | **Time** |  | [optional] |
| **value** | **Float** |  | [optional] |
| **interest_rate** | **Float** |  | [optional] |
| **is_compund_interest_rate** | **Boolean** |  | [optional] |
| **loan_type_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::LoanCreateDto.new(
  id: null,
  timestamp: null,
  loan_timestamp: null,
  payment_deadline: null,
  value: null,
  interest_rate: null,
  is_compund_interest_rate: null,
  loan_type_id: null,
  currency_id: null
)
```

