# OpenapiClient::OAuthTokenRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **client_id** | **String** |  | [optional] |
| **client_secret** | **String** |  | [optional] |
| **grant_type** | **String** |  | [optional] |
| **requested_scopes** | **String** |  | [optional] |
| **requested_enrollment** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OAuthTokenRequest.new(
  client_id: null,
  client_secret: null,
  grant_type: null,
  requested_scopes: null,
  requested_enrollment: null
)
```

