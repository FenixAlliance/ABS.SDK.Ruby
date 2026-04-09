# OpenapiClient::OpenIdConfiguration

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **issuer** | **String** |  | [optional] |
| **authorization_endpoint** | **String** |  | [optional] |
| **token_endpoint** | **String** |  | [optional] |
| **end_session_endpoint** | **String** |  | [optional] |
| **jwks_uri** | **String** |  | [optional] |
| **response_modes_supported** | **Array&lt;String&gt;** |  | [optional] |
| **response_types_supported** | **Array&lt;String&gt;** |  | [optional] |
| **scopes_supported** | **Array&lt;String&gt;** |  | [optional] |
| **subject_types_supported** | **Array&lt;String&gt;** |  | [optional] |
| **id_token_signing_alg_values_supported** | **Array&lt;String&gt;** |  | [optional] |
| **token_endpoint_auth_methods_supported** | **Array&lt;String&gt;** |  | [optional] |
| **claims_supported** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OpenIdConfiguration.new(
  issuer: null,
  authorization_endpoint: null,
  token_endpoint: null,
  end_session_endpoint: null,
  jwks_uri: null,
  response_modes_supported: null,
  response_types_supported: null,
  scopes_supported: null,
  subject_types_supported: null,
  id_token_signing_alg_values_supported: null,
  token_endpoint_auth_methods_supported: null,
  claims_supported: null
)
```

