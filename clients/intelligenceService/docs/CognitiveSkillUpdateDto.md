# OpenapiClient::CognitiveSkillUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **tool_key** | **String** |  | [optional] |
| **config_json** | **String** |  | [optional] |
| **enabled** | **Boolean** |  | [optional] |
| **tools** | [**Array&lt;CognitiveSkillToolDto&gt;**](CognitiveSkillToolDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CognitiveSkillUpdateDto.new(
  name: null,
  description: null,
  tool_key: null,
  config_json: null,
  enabled: null,
  tools: null
)
```

