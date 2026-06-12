# OpenapiClient::IEdmModel

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **schema_elements** | [**Array&lt;IEdmSchemaElement&gt;**](IEdmSchemaElement.md) |  | [optional][readonly] |
| **vocabulary_annotations** | [**Array&lt;IEdmVocabularyAnnotation&gt;**](IEdmVocabularyAnnotation.md) |  | [optional][readonly] |
| **referenced_models** | [**Array&lt;IEdmModel&gt;**](IEdmModel.md) |  | [optional][readonly] |
| **declared_namespaces** | **Array&lt;String&gt;** |  | [optional][readonly] |
| **direct_value_annotations_manager** | **Object** |  | [optional] |
| **entity_container** | [**IEdmEntityContainer**](IEdmEntityContainer.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmModel.new(
  schema_elements: null,
  vocabulary_annotations: null,
  referenced_models: null,
  declared_namespaces: null,
  direct_value_annotations_manager: null,
  entity_container: null
)
```

