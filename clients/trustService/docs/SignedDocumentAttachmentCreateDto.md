# OpenapiClient::SignedDocumentAttachmentCreateDto

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  | [optional] |
| **timestamp** | **Time** |  | [optional] |
| **signed_document_id** | **String** |  |  |
| **title** | **String** |  |  |
| **file_name** | **String** |  | [optional] |
| **content_type** | **String** |  | [optional] |
| **file_length** | **Integer** |  | [optional] |
| **hash** | **String** |  | [optional] |
| **file_upload_url** | **String** |  | [optional] |
| **storage_key** | **String** |  |  |
| **storage_provider_key** | **String** |  | [optional] |
| **attachment_role** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::SignedDocumentAttachmentCreateDto.new(
  id: null,
  timestamp: null,
  signed_document_id: null,
  title: null,
  file_name: null,
  content_type: null,
  file_length: null,
  hash: null,
  file_upload_url: null,
  storage_key: null,
  storage_provider_key: null,
  attachment_role: null
)
```

