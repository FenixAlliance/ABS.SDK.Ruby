# OpenapiClient::SignatureVerificationDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **is_valid** | **Boolean** |  | [optional] |
| **method** | **String** |  | [optional] |
| **signer_subject** | **String** |  | [optional] |
| **signer_thumbprint** | **String** |  | [optional] |
| **issues** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SignatureVerificationDto.new(
  is_valid: null,
  method: null,
  signer_subject: null,
  signer_thumbprint: null,
  issues: null
)
```

