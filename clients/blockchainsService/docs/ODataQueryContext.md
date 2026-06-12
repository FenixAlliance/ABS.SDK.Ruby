# OpenapiClient::ODataQueryContext

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **default_query_configurations** | [**DefaultQueryConfigurations**](DefaultQueryConfigurations.md) |  | [optional] |
| **model** | [**IEdmModel**](IEdmModel.md) |  | [optional] |
| **element_type** | [**IEdmType**](IEdmType.md) |  | [optional] |
| **navigation_source** | [**IEdmNavigationSource**](IEdmNavigationSource.md) |  | [optional] |
| **element_clr_type** | [**Type**](Type.md) |  | [optional] |
| **path** | [**Array&lt;ODataPathSegment&gt;**](ODataPathSegment.md) |  | [optional] |
| **request_container** | **Object** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ODataQueryContext.new(
  default_query_configurations: null,
  model: null,
  element_type: null,
  navigation_source: null,
  element_clr_type: null,
  path: null,
  request_container: null
)
```

