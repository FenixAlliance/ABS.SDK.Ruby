# OpenapiClient::Claim

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **issuer** | **String** |  | [optional][readonly] |
| **original_issuer** | **String** |  | [optional][readonly] |
| **properties** | **Hash&lt;String, String&gt;** |  | [optional][readonly] |
| **subject** | [**ClaimsIdentity**](ClaimsIdentity.md) |  | [optional] |
| **type** | **String** |  | [optional][readonly] |
| **value** | **String** |  | [optional][readonly] |
| **value_type** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Claim.new(
  issuer: null,
  original_issuer: null,
  properties: null,
  subject: null,
  type: null,
  value: null,
  value_type: null
)
```

