# OpenapiClient::OAuthApplicationUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **display_name** | **String** |  | [optional] |
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

instance = OpenapiClient::OAuthApplicationUpdateDto.new(
  display_name: null,
  client_secret: null,
  consent_type: null,
  permissions: null,
  requirements: null,
  redirect_uris: null,
  post_logout_redirect_uris: null,
  logo: null
)
```

