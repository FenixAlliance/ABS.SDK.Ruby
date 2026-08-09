# OpenapiClient::OutboxMessageDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **kind** | **String** |  | [optional] |
| **message_type** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **attempts** | **Integer** |  | [optional] |
| **max_attempts** | **Integer** |  | [optional] |
| **failure_code** | **String** |  | [optional] |
| **failure_reason** | **String** |  | [optional] |
| **idempotency_key** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **locked_by** | **String** |  | [optional] |
| **locked_until_utc** | **Time** |  | [optional] |
| **available_at_utc** | **Time** |  | [optional] |
| **created_at_utc** | **Time** |  | [optional] |
| **last_attempt_at_utc** | **Time** |  | [optional] |
| **processed_at_utc** | **Time** |  | [optional] |
| **failed_at_utc** | **Time** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::OutboxMessageDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  kind: null,
  message_type: null,
  status: null,
  attempts: null,
  max_attempts: null,
  failure_code: null,
  failure_reason: null,
  idempotency_key: null,
  correlation_id: null,
  locked_by: null,
  locked_until_utc: null,
  available_at_utc: null,
  created_at_utc: null,
  last_attempt_at_utc: null,
  processed_at_utc: null,
  failed_at_utc: null
)
```

