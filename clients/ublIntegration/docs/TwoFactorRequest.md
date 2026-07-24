# OpenapiClient::TwoFactorRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enable** | **Boolean** |  | [optional] |
| **two_factor_code** | **String** |  | [optional] |
| **reset_shared_key** | **Boolean** |  | [optional] |
| **reset_recovery_codes** | **Boolean** |  | [optional] |
| **forget_machine** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TwoFactorRequest.new(
  enable: null,
  two_factor_code: null,
  reset_shared_key: null,
  reset_recovery_codes: null,
  forget_machine: null
)
```

