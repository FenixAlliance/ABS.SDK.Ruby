# OpenapiClient::OAuthApplicationCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **display_name** | **String** |  |  |
| **client_id** | **String** |  | [optional] |
| **client_secret** | **String** |  | [optional] |
| **consent_type** | **String** |  | [optional] |
| **permissions** | **String** |  | [optional] |
| **requirements** | **String** |  | [optional] |
| **redirect_uris** | **String** |  | [optional] |
| **post_logout_redirect_uris** | **String** |  | [optional] |
| **logo** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OAuthApplicationCreateDto.new(
  id: null,
  timestamp: null,
  display_name: null,
  client_id: null,
  client_secret: null,
  consent_type: null,
  permissions: null,
  requirements: null,
  redirect_uris: null,
  post_logout_redirect_uris: null,
  logo: null
)
```

