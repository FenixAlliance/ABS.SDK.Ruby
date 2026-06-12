# OpenapiClient::FilterClause

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **expression** | [**SingleValueNode**](SingleValueNode.md) |  | [optional] |
| **range_variable** | [**RangeVariable**](RangeVariable.md) |  | [optional] |
| **item_type** | [**IEdmTypeReference**](IEdmTypeReference.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::FilterClause.new(
  expression: null,
  range_variable: null,
  item_type: null
)
```

