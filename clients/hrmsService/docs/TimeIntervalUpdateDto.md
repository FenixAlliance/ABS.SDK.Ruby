# OpenapiClient::TimeIntervalUpdateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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
| **parent_time_interval_id** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TimeIntervalUpdateDto.new(
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
  parent_time_interval_id: null
)
```

