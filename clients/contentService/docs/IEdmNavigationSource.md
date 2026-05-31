# OpenapiClient::IEdmNavigationSource

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **navigation_property_bindings** | [**Array&lt;IEdmNavigationPropertyBinding&gt;**](IEdmNavigationPropertyBinding.md) |  | [optional][readonly] |
| **path** | [**IEdmPathExpression**](IEdmPathExpression.md) |  | [optional] |
| **type** | [**IEdmType**](IEdmType.md) |  | [optional] |
| **entity_type** | [**IEdmEntityType**](IEdmEntityType.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmNavigationSource.new(
  name: null,
  navigation_property_bindings: null,
  path: null,
  type: null,
  entity_type: null
)
```

