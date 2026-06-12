# OpenapiClient::ActivityRecordDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **type** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **completed** | **Boolean** |  | [optional] |
| **due_date** | **Time** |  | [optional] |
| **activity_feed_id** | **String** |  | [optional] |
| **activity_type_id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **social_profile_id** | **String** |  | [optional] |
| **parent_activity_id** | **String** |  | [optional] |
| **in_charge_enrollment_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ActivityRecordDto.new(
  id: null,
  timestamp: null,
  type: null,
  title: null,
  description: null,
  completed: null,
  due_date: null,
  activity_feed_id: null,
  activity_type_id: null,
  tenant_id: null,
  enrollment_id: null,
  social_profile_id: null,
  parent_activity_id: null,
  in_charge_enrollment_id: null
)
```

