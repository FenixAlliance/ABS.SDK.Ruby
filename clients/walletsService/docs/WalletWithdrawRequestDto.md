# OpenapiClient::WalletWithdrawRequestDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **requested_withdraw_amount** | **Float** |  | [optional] |
| **requested_withdraw_amount_in_usd** | **Float** |  | [optional] |
| **wallet_withdraw_request_status** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **business_id** | **String** |  | [optional] |
| **wallet_account_id** | **String** |  | [optional] |
| **bank_account_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WalletWithdrawRequestDto.new(
  id: null,
  timestamp: null,
  requested_withdraw_amount: null,
  requested_withdraw_amount_in_usd: null,
  wallet_withdraw_request_status: null,
  currency_id: null,
  business_id: null,
  wallet_account_id: null,
  bank_account_id: null
)
```

