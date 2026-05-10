# OpenapiClient::PaymentTokenDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **test** | **Boolean** |  | [optional] |
| **mask** | **String** |  | [optional] |
| **token_type** | **String** |  | [optional] |
| **card_franchise** | **String** |  | [optional] |
| **card_expiration_month** | **String** |  | [optional] |
| **card_expiration_year** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **valid_until** | **Time** |  | [optional] |
| **wallet_account_id** | **String** |  | [optional] |
| **payment_gateway_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentTokenDto.new(
  id: null,
  timestamp: null,
  test: null,
  mask: null,
  token_type: null,
  card_franchise: null,
  card_expiration_month: null,
  card_expiration_year: null,
  status: null,
  valid_until: null,
  wallet_account_id: null,
  payment_gateway_id: null
)
```

