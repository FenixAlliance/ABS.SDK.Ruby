# OpenapiClient::PaymentTokenCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **mask** | **String** |  |  |
| **token_type** | **String** |  | [optional] |
| **card_franchise** | **String** |  | [optional] |
| **card_expiration_month** | **String** |  |  |
| **card_expiration_year** | **String** |  |  |
| **valid_until** | **Time** |  | [optional] |
| **payment_gateway_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentTokenCreateDto.new(
  id: null,
  timestamp: null,
  mask: null,
  token_type: null,
  card_franchise: null,
  card_expiration_month: null,
  card_expiration_year: null,
  valid_until: null,
  payment_gateway_id: null
)
```

