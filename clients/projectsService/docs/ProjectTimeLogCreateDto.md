# OpenapiClient::ProjectTimeLogCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **time_span** | **String** |  | [optional] |
| **log_date** | **Time** |  | [optional] |
| **comments** | **String** |  | [optional] |
| **project_task_id** | **String** |  |  |
| **project_period_id** | **String** |  |  |
| **project_time_log_record_type** | **String** |  | [optional] |
| **project_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ProjectTimeLogCreateDto.new(
  id: null,
  timestamp: null,
  time_span: null,
  log_date: null,
  comments: null,
  project_task_id: null,
  project_period_id: null,
  project_time_log_record_type: null,
  project_id: null
)
```

