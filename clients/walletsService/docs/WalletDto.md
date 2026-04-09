# OpenapiClient::WalletDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **balance** | **Float** |  | [optional] |
| **crypto_balance** | **Float** |  | [optional] |
| **test_mode** | **Boolean** |  | [optional] |
| **verified** | **Boolean** |  | [optional] |
| **type** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **forex_rate** | **Float** |  | [optional] |
| **balance_in_usd** | **Float** |  | [optional] |
| **main_net_ether_balance** | **Float** |  | [optional] |
| **ethereum_address** | **String** |  | [optional] |
| **ethereum_public_key** | **String** |  | [optional] |
| **ethereum_private_key** | **String** |  | [optional] |
| **rolling_reserve_percent** | **Float** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WalletDto.new(
  id: null,
  timestamp: null,
  balance: null,
  crypto_balance: null,
  test_mode: null,
  verified: null,
  type: null,
  currency_id: null,
  forex_rate: null,
  balance_in_usd: null,
  main_net_ether_balance: null,
  ethereum_address: null,
  ethereum_public_key: null,
  ethereum_private_key: null,
  rolling_reserve_percent: null
)
```

