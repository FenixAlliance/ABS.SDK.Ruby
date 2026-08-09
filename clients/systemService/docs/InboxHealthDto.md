# OpenapiClient::InboxHealthDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **enabled** | **Boolean** |  | [optional] |
| **received_count** | **Integer** |  | [optional] |
| **accepted_count** | **Integer** |  | [optional] |
| **processing_count** | **Integer** |  | [optional] |
| **retry_scheduled_count** | **Integer** |  | [optional] |
| **rejected_count** | **Integer** |  | [optional] |
| **quarantined_count** | **Integer** |  | [optional] |
| **dead_letter_count** | **Integer** |  | [optional] |
| **cancelled_count** | **Integer** |  | [optional] |
| **oldest_accepted_age_seconds** | **Float** |  | [optional] |
| **last_successful_processing_utc** | **Time** |  | [optional] |
| **successful_processing_tracked** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InboxHealthDto.new(
  enabled: null,
  received_count: null,
  accepted_count: null,
  processing_count: null,
  retry_scheduled_count: null,
  rejected_count: null,
  quarantined_count: null,
  dead_letter_count: null,
  cancelled_count: null,
  oldest_accepted_age_seconds: null,
  last_successful_processing_utc: null,
  successful_processing_tracked: null
)
```

