# OpenapiClient::SigningLogDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **type** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |
| **log_type** | **String** |  | [optional] |
| **security_event** | **String** |  | [optional] |
| **requires_attention** | **Boolean** |  | [optional] |
| **tenant_id** | **String** |  | [optional] |
| **user_id** | **String** |  | [optional] |
| **enrollment_id** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **signing_profile_id** | **String** |  | [optional] |
| **signing_certificate_id** | **String** |  | [optional] |
| **signed_document_id** | **String** |  | [optional] |
| **operation_type** | **String** |  | [optional] |
| **correlation_id** | **String** |  | [optional] |
| **input_hash** | **String** |  | [optional] |
| **output_hash** | **String** |  | [optional] |
| **provider_name** | **String** |  | [optional] |
| **result_code** | **String** |  | [optional] |
| **signing_profile_display_name** | **String** |  | [optional] |
| **signing_certificate_title** | **String** |  | [optional] |
| **signed_document_title** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SigningLogDto.new(
  id: null,
  timestamp: null,
  type: null,
  message: null,
  log_type: null,
  security_event: null,
  requires_attention: null,
  tenant_id: null,
  user_id: null,
  enrollment_id: null,
  contact_id: null,
  signing_profile_id: null,
  signing_certificate_id: null,
  signed_document_id: null,
  operation_type: null,
  correlation_id: null,
  input_hash: null,
  output_hash: null,
  provider_name: null,
  result_code: null,
  signing_profile_display_name: null,
  signing_certificate_title: null,
  signed_document_title: null
)
```

