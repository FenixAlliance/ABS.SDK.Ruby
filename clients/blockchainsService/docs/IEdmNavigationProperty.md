# OpenapiClient::IEdmNavigationProperty

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **property_kind** | **String** |  | [optional][readonly] |
| **type** | [**IEdmTypeReference**](IEdmTypeReference.md) |  | [optional] |
| **declaring_type** | [**IEdmStructuredType**](IEdmStructuredType.md) |  | [optional] |
| **partner** | [**IEdmNavigationProperty**](IEdmNavigationProperty.md) |  | [optional] |
| **on_delete** | **String** |  | [optional][readonly] |
| **contains_target** | **Boolean** |  | [optional][readonly] |
| **referential_constraint** | [**IEdmReferentialConstraint**](IEdmReferentialConstraint.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmNavigationProperty.new(
  name: null,
  property_kind: null,
  type: null,
  declaring_type: null,
  partner: null,
  on_delete: null,
  contains_target: null,
  referential_constraint: null
)
```

