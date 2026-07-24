# OpenapiClient::SigningRequestDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **signed_document_id** | **String** |  | [optional] |
| **signed_document_title** | **String** |  | [optional] |
| **frozen_source_file_upload_id** | **String** |  | [optional] |
| **source_sha256** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **routing_mode** | **String** |  | [optional] |
| **created_at_utc** | **Time** |  | [optional] |
| **sent_at_utc** | **Time** |  | [optional] |
| **completed_at_utc** | **Time** |  | [optional] |
| **expires_at_utc** | **Time** |  | [optional] |
| **voided_at_utc** | **Time** |  | [optional] |
| **voided_reason** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SigningRequestDto.new(
  id: null,
  tenant_id: null,
  signed_document_id: null,
  signed_document_title: null,
  frozen_source_file_upload_id: null,
  source_sha256: null,
  status: null,
  routing_mode: null,
  created_at_utc: null,
  sent_at_utc: null,
  completed_at_utc: null,
  expires_at_utc: null,
  voided_at_utc: null,
  voided_reason: null,
  message: null,
  correlation_id: null,
  external_reference: null
)
```

