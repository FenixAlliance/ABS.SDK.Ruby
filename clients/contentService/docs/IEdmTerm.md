# OpenapiClient::IEdmTerm

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional][readonly] |
| **schema_element_kind** | **String** |  | [optional][readonly] |
| **namespace** | **String** |  | [optional][readonly] |
| **type** | [**IEdmTypeReference**](IEdmTypeReference.md) |  | [optional] |
| **applies_to** | **String** |  | [optional][readonly] |
| **default_value** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmTerm.new(
  name: null,
  schema_element_kind: null,
  namespace: null,
  type: null,
  applies_to: null,
  default_value: null
)
```

