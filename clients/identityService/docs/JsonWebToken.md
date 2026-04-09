# OpenapiClient::JsonWebToken

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **header** | [**JsonWebTokenHeader**](JsonWebTokenHeader.md) |  | [optional] |
| **payload** | [**JsonWebTokenPayload**](JsonWebTokenPayload.md) |  | [optional] |
| **signature** | **String** |  | [optional] |
| **token_type** | **String** |  | [optional] |
| **expires_in** | **Integer** |  | [optional] |
| **access_token** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::JsonWebToken.new(
  header: null,
  payload: null,
  signature: null,
  token_type: null,
  expires_in: null,
  access_token: null
)
```

