# OpenapiClient::LeaveApplicationCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **justification** | **String** |  | [optional] |
| **approved** | **Boolean** |  | [optional] |
| **on_review** | **Boolean** |  | [optional] |
| **leave_type_id** | **String** |  |  |
| **employee_profile_id** | **String** |  |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::LeaveApplicationCreateDto.new(
  id: null,
  timestamp: null,
  justification: null,
  approved: null,
  on_review: null,
  leave_type_id: null,
  employee_profile_id: null
)
```

