# OpenapiClient::TwoFactorResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **shared_key** | **String** |  |  |
| **recovery_codes_left** | **Integer** |  |  |
| **recovery_codes** | **Array&lt;String&gt;** |  | [optional] |
| **is_two_factor_enabled** | **Boolean** |  |  |
| **is_machine_remembered** | **Boolean** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TwoFactorResponse.new(
  shared_key: null,
  recovery_codes_left: null,
  recovery_codes: null,
  is_two_factor_enabled: null,
  is_machine_remembered: null
)
```

