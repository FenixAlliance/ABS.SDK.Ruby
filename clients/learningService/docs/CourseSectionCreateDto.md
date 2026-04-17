# OpenapiClient::CourseSectionCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **name** | **String** |  |  |
| **icon** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **course_id** | **String** |  |  |
| **release_date_time** | **Time** |  | [optional] |
| **hide_from_students** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CourseSectionCreateDto.new(
  id: null,
  timestamp: null,
  name: null,
  icon: null,
  description: null,
  course_id: null,
  release_date_time: null,
  hide_from_students: null
)
```

