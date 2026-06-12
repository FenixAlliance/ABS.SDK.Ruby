# OpenapiClient::CourseUnitDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **release_date_time** | **Time** |  | [optional] |
| **content** | **String** |  | [optional] |
| **course_id** | **String** |  | [optional] |
| **course_section_id** | **String** |  | [optional] |
| **course_content_group_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **course_handouts** | [**Array&lt;CourseHandoutDto&gt;**](CourseHandoutDto.md) |  | [optional] |
| **course_assignments** | [**Array&lt;CourseAssignmentDto&gt;**](CourseAssignmentDto.md) |  | [optional] |
| **course_components** | [**Array&lt;CourseUnitComponentDto&gt;**](CourseUnitComponentDto.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CourseUnitDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  release_date_time: null,
  content: null,
  course_id: null,
  course_section_id: null,
  course_content_group_id: null,
  tenant_id: null,
  enrollment_id: null,
  course_handouts: null,
  course_assignments: null,
  course_components: null
)
```

