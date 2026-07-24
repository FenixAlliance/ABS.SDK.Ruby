# OpenapiClient::FinalizeSigningRequestDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **signed_file_upload_id** | **String** |  |  |
| **evidence_file_upload_id** | **String** |  | [optional] |
| **external_reference** | **String** |  | [optional] |
| **provider_name** | **String** |  | [optional] |
| **outcome_notes** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::FinalizeSigningRequestDto.new(
  signed_file_upload_id: null,
  evidence_file_upload_id: null,
  external_reference: null,
  provider_name: null,
  outcome_notes: null
)
```

