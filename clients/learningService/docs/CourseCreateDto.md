# OpenapiClient::CourseCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  |  |
| **sku** | **String** |  | [optional] |
| **summary** | **String** |  | [optional] |
| **code** | **String** |  | [optional] |
| **version** | **String** |  | [optional] |
| **course_category_id** | **String** |  | [optional] |
| **instructor_profile_id** | **String** |  | [optional] |
| **currency_id** | **String** |  | [optional] |
| **regular_price** | **Float** |  | [optional] |
| **max_course_enrollments** | **Integer** |  | [optional] |
| **total_effort_in_weeks** | **Integer** |  | [optional] |
| **total_hours_per_week** | **Integer** |  | [optional] |
| **total_effort_in_hours** | **Integer** |  | [optional] |
| **start_date_time** | **Time** |  | [optional] |
| **end_date_time** | **Time** |  | [optional] |
| **inscriptions_start_date_time** | **Time** |  | [optional] |
| **inscriptions_end_date_time** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CourseCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  sku: null,
  summary: null,
  code: null,
  version: null,
  course_category_id: null,
  instructor_profile_id: null,
  currency_id: null,
  regular_price: null,
  max_course_enrollments: null,
  total_effort_in_weeks: null,
  total_hours_per_week: null,
  total_effort_in_hours: null,
  start_date_time: null,
  end_date_time: null,
  inscriptions_start_date_time: null,
  inscriptions_end_date_time: null
)
```

