# OpenapiClient::WalletWithdrawRequestCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **requested_withdraw_amount** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **bank_account_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WalletWithdrawRequestCreateDto.new(
  id: null,
  timestamp: null,
  requested_withdraw_amount: null,
  currency_id: null,
  bank_account_id: null
)
```

