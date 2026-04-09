# OpenapiClient::PaymentTermUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **is_template** | **Boolean** |  | [optional] |
| **percentage** | **Float** |  | [optional] |
| **credit_days** | **Float** |  | [optional] |
| **credit_weeks** | **Float** |  | [optional] |
| **credit_months** | **Float** |  | [optional] |
| **credit_years** | **Float** |  | [optional] |
| **payment_mode_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentTermUpdateDto.new(
  name: null,
  description: null,
  is_template: null,
  percentage: null,
  credit_days: null,
  credit_weeks: null,
  credit_months: null,
  credit_years: null,
  payment_mode_id: null
)
```

