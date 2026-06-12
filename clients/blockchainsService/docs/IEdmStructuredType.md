# OpenapiClient::IEdmStructuredType

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **type_kind** | **String** |  | [optional][readonly] |
| **is_abstract** | **Boolean** |  | [optional][readonly] |
| **is_open** | **Boolean** |  | [optional][readonly] |
| **base_type** | [**IEdmStructuredType**](IEdmStructuredType.md) |  | [optional] |
| **declared_properties** | [**Array&lt;IEdmProperty&gt;**](IEdmProperty.md) |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmStructuredType.new(
  type_kind: null,
  is_abstract: null,
  is_open: null,
  base_type: null,
  declared_properties: null
)
```

