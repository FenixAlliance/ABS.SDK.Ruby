# OpenapiClient::PostingExecutionDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **posting_intent_id** | **String** |  | [optional] |
| **posting_idempotency_key** | **String** |  | [optional] |
| **intent_type** | **String** |  | [optional] |
| **posting_operation** | **String** |  | [optional] |
| **source_document_type** | **String** |  | [optional] |
| **source_document_id** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **failure_kind** | **String** |  | [optional] |
| **failure_code** | **String** |  | [optional] |
| **retryable** | **Boolean** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **causation_id** | **String** |  | [optional] |
| **received_at_utc** | **Time** |  | [optional] |
| **processing_started_at_utc** | **Time** |  | [optional] |
| **completed_at_utc** | **Time** |  | [optional] |
| **book_results** | [**Array&lt;PostingBookResultDto&gt;**](PostingBookResultDto.md) |  | [optional] |
| **failure_class** | **String** |  | [optional][readonly] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PostingExecutionDto.new(
  id: null,
  timestamp: null,
  tenant_id: null,
  enrollment_id: null,
  posting_intent_id: null,
  posting_idempotency_key: null,
  intent_type: null,
  posting_operation: null,
  source_document_type: null,
  source_document_id: null,
  status: null,
  failure_kind: null,
  failure_code: null,
  retryable: null,
  correlation_id: null,
  causation_id: null,
  received_at_utc: null,
  processing_started_at_utc: null,
  completed_at_utc: null,
  book_results: null,
  failure_class: null
)
```

