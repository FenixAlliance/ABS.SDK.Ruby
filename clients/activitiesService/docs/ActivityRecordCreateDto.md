# OpenapiClient::ActivityRecordCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **type** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **due_date** | **Time** |  | [optional] |
| **activity_feed_id** | **String** |  | [optional] |
| **activity_type_id** | **String** |  | [optional] |
| **parent_activity_id** | **String** |  | [optional] |
| **in_charge_enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ActivityRecordCreateDto.new(
  id: null,
  timestamp: null,
  type: null,
  title: null,
  description: null,
  due_date: null,
  activity_feed_id: null,
  activity_type_id: null,
  parent_activity_id: null,
  in_charge_enrollment_id: null
)
```

