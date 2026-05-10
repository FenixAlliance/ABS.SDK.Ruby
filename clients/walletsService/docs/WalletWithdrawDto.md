# OpenapiClient::WalletWithdrawDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **withdraw_status** | **String** |  | [optional] |
| **wallet_account_id** | **String** |  | [optional] |
| **wallet_withdraw_request_id** | **String** |  | [optional] |
| **balance_before_withdraw** | **Float** |  | [optional] |
| **balance_after_withdraw** | **Float** |  | [optional] |
| **withdrawed_amount** | **Float** |  | [optional] |
| **currency_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WalletWithdrawDto.new(
  id: null,
  timestamp: null,
  withdraw_status: null,
  wallet_account_id: null,
  wallet_withdraw_request_id: null,
  balance_before_withdraw: null,
  balance_after_withdraw: null,
  withdrawed_amount: null,
  currency_id: null
)
```

