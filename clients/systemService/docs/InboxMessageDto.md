# OpenapiClient::InboxMessageDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **source_system** | **String** |  | [optional] |
| **source_registration_id** | **String** |  | [optional] |
| **external_message_id** | **String** |  | [optional] |
| **deduplication_key** | **String** |  | [optional] |
| **deduplication_signature** | **String** |  | [optional] |
| **payload_digest** | **String** |  | [optional] |
| **delivery_count** | **Integer** |  | [optional] |
| **last_duplicate_received_at_utc** | **Time** |  | [optional] |
| **message_type** | **String** |  | [optional] |
| **version** | **String** |  | [optional] |
| **content_type** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **attempts** | **Integer** |  | [optional] |
| **max_attempts** | **Integer** |  | [optional] |
| **verification_status** | **String** |  | [optional] |
| **verification_profile** | **String** |  | [optional] |
| **verification_algorithm** | **String** |  | [optional] |
| **verified_at_utc** | **Time** |  | [optional] |
| **generation** | **Integer** |  | [optional] |
| **replay_count** | **Integer** |  | [optional] |
| **original_inbox_message_id** | **String** |  | [optional] |
| **failure_code** | **String** |  | [optional] |
| **failure_reason** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **causation_id** | **String** |  | [optional] |
| **locked_by** | **String** |  | [optional] |
| **locked_until_utc** | **Time** |  | [optional] |
| **available_at_utc** | **Time** |  | [optional] |
| **received_at_utc** | **Time** |  | [optional] |
| **created_at_utc** | **Time** |  | [optional] |
| **last_attempt_at_utc** | **Time** |  | [optional] |
| **processed_at_utc** | **Time** |  | [optional] |
| **failed_at_utc** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::InboxMessageDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  source_system: null,
  source_registration_id: null,
  external_message_id: null,
  deduplication_key: null,
  deduplication_signature: null,
  payload_digest: null,
  delivery_count: null,
  last_duplicate_received_at_utc: null,
  message_type: null,
  version: null,
  content_type: null,
  status: null,
  attempts: null,
  max_attempts: null,
  verification_status: null,
  verification_profile: null,
  verification_algorithm: null,
  verified_at_utc: null,
  generation: null,
  replay_count: null,
  original_inbox_message_id: null,
  failure_code: null,
  failure_reason: null,
  correlation_id: null,
  causation_id: null,
  locked_by: null,
  locked_until_utc: null,
  available_at_utc: null,
  received_at_utc: null,
  created_at_utc: null,
  last_attempt_at_utc: null,
  processed_at_utc: null,
  failed_at_utc: null
)
```

