# OpenapiClient::SelectExpandQueryOption

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **context** | [**ODataQueryContext**](ODataQueryContext.md) |  | [optional] |
| **raw_select** | **String** |  | [optional][readonly] |
| **raw_expand** | **String** |  | [optional][readonly] |
| **compute** | [**ComputeQueryOption**](ComputeQueryOption.md) |  | [optional] |
| **validator** | **Object** |  | [optional] |
| **select_expand_clause** | [**SelectExpandClause**](SelectExpandClause.md) |  | [optional] |
| **levels_max_literal_expansion_depth** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SelectExpandQueryOption.new(
  context: null,
  raw_select: null,
  raw_expand: null,
  compute: null,
  validator: null,
  select_expand_clause: null,
  levels_max_literal_expansion_depth: null
)
```

