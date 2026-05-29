# OpenapiClient::AuthResult

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_id** | **Object** |  | [optional] |
| **tenant_id** | **Object** |  | [optional] |
| **portal_id** | **Object** |  | [optional] |
| **application_id** | **Object** |  | [optional] |
| **enrollment_id** | **Object** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **scopes** | **Array&lt;String&gt;** |  | [optional] |
| **error** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::AuthResult.new(
  user_id: null,
  tenant_id: null,
  portal_id: null,
  application_id: null,
  enrollment_id: null,
  correlation_id: null,
  scopes: null,
  error: null
)
```

