# OpenapiClient::ActivityRecordUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **type** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **completed** | **Boolean** |  | [optional] |
| **due_date** | **Time** |  | [optional] |
| **activity_type_id** | **String** |  | [optional] |
| **parent_activity_id** | **String** |  | [optional] |
| **in_charge_enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ActivityRecordUpdateDto.new(
  type: null,
  title: null,
  description: null,
  completed: null,
  due_date: null,
  activity_type_id: null,
  parent_activity_id: null,
  in_charge_enrollment_id: null
)
```

