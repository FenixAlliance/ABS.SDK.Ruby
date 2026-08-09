# OpenapiClient::CognitiveSkillDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **tool_key** | **String** |  | [optional] |
| **config_json** | **String** |  | [optional] |
| **enabled** | **Boolean** |  | [optional] |
| **tools** | [**Array&lt;CognitiveSkillToolDto&gt;**](CognitiveSkillToolDto.md) |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CognitiveSkillDto.new(
  id: null,
  timestamp: null,
  name: null,
  description: null,
  tool_key: null,
  config_json: null,
  enabled: null,
  tools: null,
  tenant_id: null,
  enrollment_id: null
)
```

