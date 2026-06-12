# OpenapiClient::ClaimsPrincipal

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **claims** | [**Array&lt;Claim&gt;**](Claim.md) |  | [optional][readonly] |
| **identities** | [**Array&lt;ClaimsIdentity&gt;**](ClaimsIdentity.md) |  | [optional][readonly] |
| **identity** | [**IIdentity**](IIdentity.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ClaimsPrincipal.new(
  claims: null,
  identities: null,
  identity: null
)
```

