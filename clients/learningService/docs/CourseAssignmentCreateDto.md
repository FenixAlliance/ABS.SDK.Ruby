# OpenapiClient::CourseAssignmentCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **instructions** | **String** |  | [optional] |
| **points** | **Float** |  | [optional] |
| **course_id** | **String** |  |  |
| **business_id** | **String** |  |  |
| **course_unit_id** | **String** |  | [optional] |
| **course_cohort_id** | **String** |  | [optional] |
| **course_assignment_type_id** | **String** |  | [optional] |
| **due_date_time** | **Time** |  | [optional] |
| **asign_to_all_cohorts** | **Boolean** |  | [optional] |
| **resources** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CourseAssignmentCreateDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  instructions: null,
  points: null,
  course_id: null,
  business_id: null,
  course_unit_id: null,
  course_cohort_id: null,
  course_assignment_type_id: null,
  due_date_time: null,
  asign_to_all_cohorts: null,
  resources: null
)
```

