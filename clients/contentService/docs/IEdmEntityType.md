# OpenapiClient::IEdmEntityType

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **type_kind** | **String** |  | [optional][readonly] |
| **name** | **String** |  | [optional][readonly] |
| **is_abstract** | **Boolean** |  | [optional][readonly] |
| **is_open** | **Boolean** |  | [optional][readonly] |
| **base_type** | [**IEdmStructuredType**](IEdmStructuredType.md) |  | [optional] |
| **declared_properties** | [**Array&lt;IEdmProperty&gt;**](IEdmProperty.md) |  | [optional][readonly] |
| **schema_element_kind** | **String** |  | [optional][readonly] |
| **namespace** | **String** |  | [optional][readonly] |
| **declared_key** | [**Array&lt;IEdmStructuralProperty&gt;**](IEdmStructuralProperty.md) |  | [optional][readonly] |
| **has_stream** | **Boolean** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmEntityType.new(
  type_kind: null,
  name: null,
  is_abstract: null,
  is_open: null,
  base_type: null,
  declared_properties: null,
  schema_element_kind: null,
  namespace: null,
  declared_key: null,
  has_stream: null
)
```

