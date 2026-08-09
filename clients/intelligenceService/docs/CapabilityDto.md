# OpenapiClient::CapabilityDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **key** | **String** |  | [optional] |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **category** | **String** |  | [optional] |
| **effect** | **String** |  | [optional] |
| **risks** | **Array&lt;String&gt;** |  | [optional] |
| **surfaces** | **Array&lt;String&gt;** |  | [optional] |
| **required_permission** | **String** |  | [optional] |
| **available** | **Boolean** |  | [optional] |
| **denied_reason** | **String** |  | [optional] |
| **version** | **String** |  | [optional] |
| **input_schema** | **Hash&lt;String, String&gt;** |  | [optional] |
| **output_schema** | **Hash&lt;String, String&gt;** |  | [optional] |
| **is_output_collection** | **Boolean** |  | [optional] |
| **required_inputs** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CapabilityDto.new(
  id: null,
  timestamp: null,
  key: null,
  name: null,
  description: null,
  category: null,
  effect: null,
  risks: null,
  surfaces: null,
  required_permission: null,
  available: null,
  denied_reason: null,
  version: null,
  input_schema: null,
  output_schema: null,
  is_output_collection: null,
  required_inputs: null
)
```

