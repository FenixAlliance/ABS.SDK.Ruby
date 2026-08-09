# OpenapiClient::UserAdminUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email** | **String** |  | [optional] |
| **user_name** | **String** |  | [optional] |
| **handler** | **String** |  | [optional] |
| **name** | **String** |  | [optional] |
| **last_name** | **String** |  | [optional] |
| **public_name** | **String** |  | [optional] |
| **about** | **String** |  | [optional] |
| **two_factor_enabled** | **Boolean** |  | [optional] |
| **lockout_enabled** | **Boolean** |  | [optional] |
| **lockout_end** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::UserAdminUpdateDto.new(
  email: null,
  user_name: null,
  handler: null,
  name: null,
  last_name: null,
  public_name: null,
  about: null,
  two_factor_enabled: null,
  lockout_enabled: null,
  lockout_end: null
)
```

