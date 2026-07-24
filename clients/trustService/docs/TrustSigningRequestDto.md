# OpenapiClient::TrustSigningRequestDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **signed_document_id** | **String** |  | [optional] |
| **signing_profile_id** | **String** |  | [optional] |
| **signing_certificate_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **requested_format** | **String** |  | [optional] |
| **requested_purpose** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **source_storage_object_id** | **String** |  | [optional] |
| **source_sha256** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |
| **dry_run** | **Boolean** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TrustSigningRequestDto.new(
  signed_document_id: null,
  signing_profile_id: null,
  signing_certificate_id: null,
  contact_id: null,
  requested_format: null,
  requested_purpose: null,
  correlation_id: null,
  source_storage_object_id: null,
  source_sha256: null,
  external_reference: null,
  dry_run: null
)
```

