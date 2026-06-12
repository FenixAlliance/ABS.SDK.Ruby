# OpenapiClient::IEdmStructuralProperty

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **property_kind** | **String** |  | [optional][readonly] |
| **type** | [**IEdmTypeReference**](IEdmTypeReference.md) |  | [optional] |
| **declaring_type** | [**IEdmStructuredType**](IEdmStructuredType.md) |  | [optional] |
| **default_value_string** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmStructuralProperty.new(
  name: null,
  property_kind: null,
  type: null,
  declaring_type: null,
  default_value_string: null
)
```

