# OpenapiClient::OrderByQueryOption

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **context** | [**ODataQueryContext**](ODataQueryContext.md) |  | [optional] |
| **order_by_nodes** | [**Array&lt;OrderByNode&gt;**](OrderByNode.md) |  | [optional][readonly] |
| **raw_value** | **String** |  | [optional] |
| **validator** | **Object** |  | [optional] |
| **compute** | [**ComputeQueryOption**](ComputeQueryOption.md) |  | [optional] |
| **order_by_clause** | [**OrderByClause**](OrderByClause.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OrderByQueryOption.new(
  context: null,
  order_by_nodes: null,
  raw_value: null,
  validator: null,
  compute: null,
  order_by_clause: null
)
```

