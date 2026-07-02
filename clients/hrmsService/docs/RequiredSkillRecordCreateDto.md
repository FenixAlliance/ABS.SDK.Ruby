# OpenapiClient::RequiredSkillRecordCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **skill_id** | **String** |  |  |
| **job_offer_id** | **String** |  | [optional] |
| **employer_profile_id** | **String** |  | [optional] |
| **experience_in_years** | **Integer** |  | [optional] |
| **priority** | **Float** |  | [optional] |
| **required_skill_record_type** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RequiredSkillRecordCreateDto.new(
  id: null,
  timestamp: null,
  skill_id: null,
  job_offer_id: null,
  employer_profile_id: null,
  experience_in_years: null,
  priority: null,
  required_skill_record_type: null
)
```

