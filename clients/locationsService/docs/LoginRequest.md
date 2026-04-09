# OpenapiClient::LoginRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email** | **String** |  |  |
| **password** | **String** |  |  |
| **two_factor_code** | **String** |  | [optional] |
| **two_factor_recovery_code** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::LoginRequest.new(
  email: null,
  password: null,
  two_factor_code: null,
  two_factor_recovery_code: null
)
```

