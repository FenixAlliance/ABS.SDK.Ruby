# OpenapiClient::PaymentChargebackDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **request_date** | **Time** |  | [optional] |
| **payment_id** | **String** |  | [optional] |
| **bank_profile_id** | **String** |  | [optional] |
| **bank_profile_name** | **String** |  | [optional] |
| **total_fees** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentChargebackDto.new(
  id: null,
  timestamp: null,
  request_date: null,
  payment_id: null,
  bank_profile_id: null,
  bank_profile_name: null,
  total_fees: null
)
```

