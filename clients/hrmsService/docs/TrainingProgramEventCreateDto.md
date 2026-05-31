# OpenapiClient::TrainingProgramEventCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **start** | **Time** |  |  |
| **_end** | **Time** |  |  |
| **is_break** | **Boolean** |  | [optional] |
| **occust_on_monday** | **Boolean** |  | [optional] |
| **occust_on_tuesday** | **Boolean** |  | [optional] |
| **occust_on_wednesday** | **Boolean** |  | [optional] |
| **occust_on_thursday** | **Boolean** |  | [optional] |
| **occust_on_friday** | **Boolean** |  | [optional] |
| **occust_on_saturday** | **Boolean** |  | [optional] |
| **occust_on_sunday** | **Boolean** |  | [optional] |
| **repeat_every** | **Integer** |  | [optional] |
| **repetition_criteria** | **String** |  | [optional] |
| **recurrence_start** | **Time** |  | [optional] |
| **recurrence_end** | **Time** |  | [optional] |
| **day_of_the_week** | **String** |  | [optional] |
| **schedule_id** | **String** |  | [optional] |
| **parent_time_interval_id** | **String** |  | [optional] |
| **training_program_id** | **String** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TrainingProgramEventCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  start: null,
  _end: null,
  is_break: null,
  occust_on_monday: null,
  occust_on_tuesday: null,
  occust_on_wednesday: null,
  occust_on_thursday: null,
  occust_on_friday: null,
  occust_on_saturday: null,
  occust_on_sunday: null,
  repeat_every: null,
  repetition_criteria: null,
  recurrence_start: null,
  recurrence_end: null,
  day_of_the_week: null,
  schedule_id: null,
  parent_time_interval_id: null,
  training_program_id: null
)
```

