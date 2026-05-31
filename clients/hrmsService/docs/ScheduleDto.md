# OpenapiClient::ScheduleDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **name** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **disabled** | **Boolean** |  | [optional] |
| **sunday** | **Boolean** |  | [optional] |
| **monday** | **Boolean** |  | [optional] |
| **tuesday** | **Boolean** |  | [optional] |
| **wednesday** | **Boolean** |  | [optional] |
| **thursday** | **Boolean** |  | [optional] |
| **friday** | **Boolean** |  | [optional] |
| **saturday** | **Boolean** |  | [optional] |
| **unique_interval** | **Boolean** |  | [optional] |
| **is24x7_interval** | **Boolean** |  | [optional] |
| **start** | **Time** |  | [optional] |
| **_end** | **Time** |  | [optional] |
| **timezone_id** | **String** |  | [optional] |
| **fiscal_year_id** | **String** |  | [optional] |
| **holiday_schedule_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ScheduleDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  name: null,
  description: null,
  disabled: null,
  sunday: null,
  monday: null,
  tuesday: null,
  wednesday: null,
  thursday: null,
  friday: null,
  saturday: null,
  unique_interval: null,
  is24x7_interval: null,
  start: null,
  _end: null,
  timezone_id: null,
  fiscal_year_id: null,
  holiday_schedule_id: null
)
```

