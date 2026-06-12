# OpenapiClient::CourseAssignmentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **instructions** | **String** |  | [optional] |
| **points** | **Float** |  | [optional] |
| **due_date_time** | **Time** |  | [optional] |
| **course_id** | **String** |  | [optional] |
| **course_unit_id** | **String** |  | [optional] |
| **course_section_id** | **String** |  | [optional] |
| **course_cohort_id** | **String** |  | [optional] |
| **course_assignment_type_id** | **String** |  | [optional] |
| **asign_to_all_cohorts** | **Boolean** |  | [optional] |
| **resources** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CourseAssignmentDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  instructions: null,
  points: null,
  due_date_time: null,
  course_id: null,
  course_unit_id: null,
  course_section_id: null,
  course_cohort_id: null,
  course_assignment_type_id: null,
  asign_to_all_cohorts: null,
  resources: null,
  tenant_id: null,
  enrollment_id: null
)
```

