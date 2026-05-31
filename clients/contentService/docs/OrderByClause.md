# OpenapiClient::OrderByClause

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **then_by** | [**OrderByClause**](OrderByClause.md) |  | [optional] |
| **expression** | [**SingleValueNode**](SingleValueNode.md) |  | [optional] |
| **direction** | **String** |  | [optional] |
| **range_variable** | [**RangeVariable**](RangeVariable.md) |  | [optional] |
| **item_type** | [**IEdmTypeReference**](IEdmTypeReference.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OrderByClause.new(
  then_by: null,
  expression: null,
  direction: null,
  range_variable: null,
  item_type: null
)
```

