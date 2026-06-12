# OpenapiClient::IEdmVocabularyAnnotation

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **qualifier** | **String** |  | [optional][readonly] |
| **term** | [**IEdmTerm**](IEdmTerm.md) |  | [optional] |
| **target** | **Object** |  | [optional] |
| **value** | [**IEdmExpression**](IEdmExpression.md) |  | [optional] |
| **uses_default** | **Boolean** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::IEdmVocabularyAnnotation.new(
  qualifier: null,
  term: null,
  target: null,
  value: null,
  uses_default: null
)
```

