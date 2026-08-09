# OpenapiClient::OutboxHealthDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enabled** | **Boolean** |  | [optional] |
| **pending_count** | **Integer** |  | [optional] |
| **processing_count** | **Integer** |  | [optional] |
| **failed_count** | **Integer** |  | [optional] |
| **dead_letter_count** | **Integer** |  | [optional] |
| **oldest_pending_age_seconds** | **Float** |  | [optional] |
| **last_successful_dispatch_utc** | **Time** |  | [optional] |
| **successful_dispatch_tracked** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OutboxHealthDto.new(
  enabled: null,
  pending_count: null,
  processing_count: null,
  failed_count: null,
  dead_letter_count: null,
  oldest_pending_age_seconds: null,
  last_successful_dispatch_utc: null,
  successful_dispatch_tracked: null
)
```

