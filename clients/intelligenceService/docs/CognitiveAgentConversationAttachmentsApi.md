# OpenapiClient::CognitiveAgentConversationAttachmentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**upload_cognitive_agent_conversation_attachment_async**](CognitiveAgentConversationAttachmentsApi.md#upload_cognitive_agent_conversation_attachment_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Attachments | Upload an attachment to a cognitive agent conversation |


## upload_cognitive_agent_conversation_attachment_async

> <ConversationAttachmentUploadResultDtoEnvelope> upload_cognitive_agent_conversation_attachment_async(tenant_id, agent_id, conversation_id, opts)

Upload an attachment to a cognitive agent conversation

Uploads a file into the acting user's OWN conversation attachment store, scanned and catalogued through the storage spine. A conversation the caller does not own returns 404. The response carries the new file's id, name, content type and length; the chat UI passes that id as an AttachmentFileIds entry when it sends the referencing user turn.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  file: File.new('/path/to/some/file') # File | 
}

begin
  # Upload an attachment to a cognitive agent conversation
  result = api_instance.upload_cognitive_agent_conversation_attachment_async(tenant_id, agent_id, conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationAttachmentsApi->upload_cognitive_agent_conversation_attachment_async: #{e}"
end
```

#### Using the upload_cognitive_agent_conversation_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ConversationAttachmentUploadResultDtoEnvelope>, Integer, Hash)> upload_cognitive_agent_conversation_attachment_async_with_http_info(tenant_id, agent_id, conversation_id, opts)

```ruby
begin
  # Upload an attachment to a cognitive agent conversation
  data, status_code, headers = api_instance.upload_cognitive_agent_conversation_attachment_async_with_http_info(tenant_id, agent_id, conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ConversationAttachmentUploadResultDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationAttachmentsApi->upload_cognitive_agent_conversation_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **conversation_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |

### Return type

[**ConversationAttachmentUploadResultDtoEnvelope**](ConversationAttachmentUploadResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, application/xml

