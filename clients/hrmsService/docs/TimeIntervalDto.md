# OpenapiClient::TimeIntervalDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **title** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **is_break** | **Boolean** |  | [optional] |
| **occust_on_monday** | **Boolean** |  | [optional] |
| **occust_on_tuesday** | **Boolean** |  | [optional] |
| **occust_on_wednesday** | **Boolean** |  | [optional] |
| **occust_on_thursday** | **Boolean** |  | [optional] |
| **occust_on_friday** | **Boolean** |  | [optional] |
| **occust_on_saturday** | **Boolean** |  | [optional] |
| **occust_on_sunday** | **Boolean** |  | [optional] |
| **start** | **Time** |  | [optional] |
| **_end** | **Time** |  | [optional] |
| **repeat_every** | **Integer** |  | [optional] |
| **schedule_id** | **String** |  | [optional] |
| **parent_time_interval_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TimeIntervalDto.new(
  id: null,
  timestamp: null,
  title: null,
  description: null,
  is_break: null,
  occust_on_monday: null,
  occust_on_tuesday: null,
  occust_on_wednesday: null,
  occust_on_thursday: null,
  occust_on_friday: null,
  occust_on_saturday: null,
  occust_on_sunday: null,
  start: null,
  _end: null,
  repeat_every: null,
  schedule_id: null,
  parent_time_interval_id: null
)
```

