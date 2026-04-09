# OpenapiClient::CourseProblemSetCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **overall_score** | **Float** |  | [optional] |
| **course_id** | **String** |  |  |
| **business_id** | **String** |  |  |
| **course_unit_id** | **String** |  | [optional] |
| **course_grading_rubric_id** | **String** |  | [optional] |
| **release_date_time** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CourseProblemSetCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  overall_score: null,
  course_id: null,
  business_id: null,
  course_unit_id: null,
  course_grading_rubric_id: null,
  release_date_time: null
)
```

