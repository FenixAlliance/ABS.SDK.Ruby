# OpenapiClient::PaymentRefundDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **payment_id** | **String** |  | [optional] |
| **wallet_account_id** | **String** |  | [optional] |
| **refund_request_id** | **String** |  | [optional] |
| **total_fees** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentRefundDto.new(
  id: null,
  timestamp: null,
  payment_id: null,
  wallet_account_id: null,
  refund_request_id: null,
  total_fees: null
)
```

