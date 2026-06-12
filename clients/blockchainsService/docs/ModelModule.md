# OpenapiClient::ModelModule

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **assembly** | [**Assembly**](Assembly.md) |  | [optional] |
| **fully_qualified_name** | **String** |  | [optional][readonly] |
| **name** | **String** |  | [optional][readonly] |
| **md_stream_version** | **Integer** |  | [optional][readonly] |
| **module_version_id** | **String** |  | [optional][readonly] |
| **scope_name** | **String** |  | [optional][readonly] |
| **module_handle** | [**ModuleHandle**](ModuleHandle.md) |  | [optional] |
| **custom_attributes** | [**Array&lt;CustomAttributeData&gt;**](CustomAttributeData.md) |  | [optional][readonly] |
| **metadata_token** | **Integer** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ModelModule.new(
  assembly: null,
  fully_qualified_name: null,
  name: null,
  md_stream_version: null,
  module_version_id: null,
  scope_name: null,
  module_handle: null,
  custom_attributes: null,
  metadata_token: null
)
```

