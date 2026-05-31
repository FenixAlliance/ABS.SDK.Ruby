# OpenapiClient::IEdmProperty

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **property_kind** | **String** |  | [optional][readonly] |
| **type** | [**IEdmTypeReference**](IEdmTypeReference.md) |  | [optional] |
| **declaring_type** | [**IEdmStructuredType**](IEdmStructuredType.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmProperty.new(
  name: null,
  property_kind: null,
  type: null,
  declaring_type: null
)
```

