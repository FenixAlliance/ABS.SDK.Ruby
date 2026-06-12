# OpenapiClient::ClaimsIdentity

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **authentication_type** | **String** |  | [optional][readonly] |
| **is_authenticated** | **Boolean** |  | [optional][readonly] |
| **actor** | [**ClaimsIdentity**](ClaimsIdentity.md) |  | [optional] |
| **bootstrap_context** | **Object** |  | [optional] |
| **claims** | [**Array&lt;Claim&gt;**](Claim.md) |  | [optional][readonly] |
| **label** | **String** |  | [optional] |
| **name** | **String** |  | [optional][readonly] |
| **name_claim_type** | **String** |  | [optional][readonly] |
| **role_claim_type** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ClaimsIdentity.new(
  authentication_type: null,
  is_authenticated: null,
  actor: null,
  bootstrap_context: null,
  claims: null,
  label: null,
  name: null,
  name_claim_type: null,
  role_claim_type: null
)
```

