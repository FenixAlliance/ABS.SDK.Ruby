# OpenapiClient::SignedDocumentDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **signed** | **Boolean** |  | [optional] |
| **url** | **String** |  | [optional] |
| **type** | **String** |  | [optional] |
| **title** | **String** |  | [optional] |
| **content_type** | **String** |  | [optional] |
| **file_length_in_bits** | **Integer** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **user_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **document_standard** | **String** |  | [optional] |
| **trust_document_type** | **String** |  | [optional] |
| **signing_status** | **String** |  | [optional] |
| **verification_status** | **String** |  | [optional] |
| **signed_at_utc** | **Time** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |
| **source_storage_object_id** | **String** |  | [optional] |
| **source_sha256** | **String** |  | [optional] |
| **signed_storage_object_id** | **String** |  | [optional] |
| **signed_sha256** | **String** |  | [optional] |
| **evidence_storage_object_id** | **String** |  | [optional] |
| **evidence_sha256** | **String** |  | [optional] |
| **primary_file_upload_id** | **String** |  | [optional] |
| **frozen_source_file_upload_id** | **String** |  | [optional] |
| **signed_file_upload_id** | **String** |  | [optional] |
| **evidence_file_upload_id** | **String** |  | [optional] |
| **lock_state** | **String** |  | [optional] |
| **graphical_representation_file_upload_id** | **String** |  | [optional] |
| **graphical_representation_storage_object_id** | **String** |  | [optional] |
| **graphical_representation_sha256** | **String** |  | [optional] |
| **graphical_representation_content_type** | **String** |  | [optional] |
| **graphical_representation_generated_at_utc** | **Time** |  | [optional] |
| **contact_name** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SignedDocumentDto.new(
  id: null,
  timestamp: null,
  signed: null,
  url: null,
  type: null,
  title: null,
  content_type: null,
  file_length_in_bits: null,
  tenant_id: null,
  contact_id: null,
  user_id: null,
  enrollment_id: null,
  document_standard: null,
  trust_document_type: null,
  signing_status: null,
  verification_status: null,
  signed_at_utc: null,
  correlation_id: null,
  external_reference: null,
  source_storage_object_id: null,
  source_sha256: null,
  signed_storage_object_id: null,
  signed_sha256: null,
  evidence_storage_object_id: null,
  evidence_sha256: null,
  primary_file_upload_id: null,
  frozen_source_file_upload_id: null,
  signed_file_upload_id: null,
  evidence_file_upload_id: null,
  lock_state: null,
  graphical_representation_file_upload_id: null,
  graphical_representation_storage_object_id: null,
  graphical_representation_sha256: null,
  graphical_representation_content_type: null,
  graphical_representation_generated_at_utc: null,
  contact_name: null
)
```

