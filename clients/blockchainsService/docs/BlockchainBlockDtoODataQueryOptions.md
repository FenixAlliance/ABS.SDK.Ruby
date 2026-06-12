# OpenapiClient::BlockchainBlockDtoODataQueryOptions

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request** | [**HttpRequest**](HttpRequest.md) |  | [optional] |
| **context** | [**ODataQueryContext**](ODataQueryContext.md) |  | [optional] |
| **raw_values** | [**ODataRawQueryOptions**](ODataRawQueryOptions.md) |  | [optional] |
| **select_expand** | [**SelectExpandQueryOption**](SelectExpandQueryOption.md) |  | [optional] |
| **apply** | [**ApplyQueryOption**](ApplyQueryOption.md) |  | [optional] |
| **compute** | [**ComputeQueryOption**](ComputeQueryOption.md) |  | [optional] |
| **filter** | [**FilterQueryOption**](FilterQueryOption.md) |  | [optional] |
| **search** | [**SearchQueryOption**](SearchQueryOption.md) |  | [optional] |
| **order_by** | [**OrderByQueryOption**](OrderByQueryOption.md) |  | [optional] |
| **skip** | [**SkipQueryOption**](SkipQueryOption.md) |  | [optional] |
| **skip_token** | [**SkipTokenQueryOption**](SkipTokenQueryOption.md) |  | [optional] |
| **top** | [**TopQueryOption**](TopQueryOption.md) |  | [optional] |
| **count** | [**CountQueryOption**](CountQueryOption.md) |  | [optional] |
| **validator** | **Object** |  | [optional] |
| **if_match** | [**BlockchainBlockDtoETag**](BlockchainBlockDtoETag.md) |  | [optional] |
| **if_none_match** | [**BlockchainBlockDtoETag**](BlockchainBlockDtoETag.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::BlockchainBlockDtoODataQueryOptions.new(
  request: null,
  context: null,
  raw_values: null,
  select_expand: null,
  apply: null,
  compute: null,
  filter: null,
  search: null,
  order_by: null,
  skip: null,
  skip_token: null,
  top: null,
  count: null,
  validator: null,
  if_match: null,
  if_none_match: null
)
```

