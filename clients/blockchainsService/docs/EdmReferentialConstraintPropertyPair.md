# OpenapiClient::EdmReferentialConstraintPropertyPair

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **dependent_property** | [**IEdmStructuralProperty**](IEdmStructuralProperty.md) |  | [optional] |
| **principal_property** | [**IEdmStructuralProperty**](IEdmStructuralProperty.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::EdmReferentialConstraintPropertyPair.new(
  dependent_property: null,
  principal_property: null
)
```

