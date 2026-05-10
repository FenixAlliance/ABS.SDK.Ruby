# OpenapiClient::PaymentTokenUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **mask** | **String** |  | [optional] |
| **token_type** | **String** |  | [optional] |
| **card_franchise** | **String** |  | [optional] |
| **card_expiration_month** | **String** |  | [optional] |
| **card_expiration_year** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **valid_until** | **Time** |  | [optional] |
| **payment_gateway_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PaymentTokenUpdateDto.new(
  mask: null,
  token_type: null,
  card_franchise: null,
  card_expiration_month: null,
  card_expiration_year: null,
  status: null,
  valid_until: null,
  payment_gateway_id: null
)
```

