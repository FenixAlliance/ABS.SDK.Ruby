# OpenapiClient::PaymentTermDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **is_template** | **Boolean** |  | [optional] |
| **percentage** | **Float** |  | [optional] |
| **credit_days** | **Float** |  | [optional] |
| **credit_weeks** | **Float** |  | [optional] |
| **credit_months** | **Float** |  | [optional] |
| **credit_years** | **Float** |  | [optional] |
| **payment_mode_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentTermDto.new(
  id: null,
  timestamp: null,
  name: null,
  description: null,
  is_template: null,
  percentage: null,
  credit_days: null,
  credit_weeks: null,
  credit_months: null,
  credit_years: null,
  payment_mode_id: null,
  tenant_id: null,
  enrollment_id: null
)
```

