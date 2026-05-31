# OpenapiClient::FilterQueryOption

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **context** | [**ODataQueryContext**](ODataQueryContext.md) |  | [optional] |
| **validator** | **Object** |  | [optional] |
| **compute** | [**ComputeQueryOption**](ComputeQueryOption.md) |  | [optional] |
| **filter_clause** | [**FilterClause**](FilterClause.md) |  | [optional] |
| **raw_value** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::FilterQueryOption.new(
  context: null,
  validator: null,
  compute: null,
  filter_clause: null,
  raw_value: null
)
```

