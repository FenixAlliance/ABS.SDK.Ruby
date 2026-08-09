# OpenapiClient::CognitiveAgentMessagesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_cognitive_agent_message_by_id_async**](CognitiveAgentMessagesApi.md#get_cognitive_agent_message_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Messages/{id} | Get a cognitive agent conversation message by ID |
| [**get_cognitive_agent_messages_async**](CognitiveAgentMessagesApi.md#get_cognitive_agent_messages_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Messages | Get all messages for a cognitive agent conversation |
| [**get_cognitive_agent_messages_count_async**](CognitiveAgentMessagesApi.md#get_cognitive_agent_messages_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{conversationId}/Messages/Count | Get message count for a cognitive agent conversation |


## get_cognitive_agent_message_by_id_async

> <CognitiveAgentMessageDtoEnvelope> get_cognitive_agent_message_by_id_async(tenant_id, agent_id, conversation_id, id, opts)

Get a cognitive agent conversation message by ID

Retrieves a specific durable message of a conversation by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentMessagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cognitive agent conversation message by ID
  result = api_instance.get_cognitive_agent_message_by_id_async(tenant_id, agent_id, conversation_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentMessagesApi->get_cognitive_agent_message_by_id_async: #{e}"
end
```

#### Using the get_cognitive_agent_message_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentMessageDtoEnvelope>, Integer, Hash)> get_cognitive_agent_message_by_id_async_with_http_info(tenant_id, agent_id, conversation_id, id, opts)

```ruby
begin
  # Get a cognitive agent conversation message by ID
  data, status_code, headers = api_instance.get_cognitive_agent_message_by_id_async_with_http_info(tenant_id, agent_id, conversation_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentMessageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentMessagesApi->get_cognitive_agent_message_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **conversation_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CognitiveAgentMessageDtoEnvelope**](CognitiveAgentMessageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_agent_messages_async

> <CognitiveAgentMessageDtoListEnvelope> get_cognitive_agent_messages_async(tenant_id, agent_id, conversation_id, opts)

Get all messages for a cognitive agent conversation

Retrieves all durable messages for the specified conversation, agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentMessagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_message_dto_collection_query_parameters: OpenapiClient::CognitiveAgentMessageDtoCollectionQueryParameters.new # CognitiveAgentMessageDtoCollectionQueryParameters | 
}

begin
  # Get all messages for a cognitive agent conversation
  result = api_instance.get_cognitive_agent_messages_async(tenant_id, agent_id, conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentMessagesApi->get_cognitive_agent_messages_async: #{e}"
end
```

#### Using the get_cognitive_agent_messages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentMessageDtoListEnvelope>, Integer, Hash)> get_cognitive_agent_messages_async_with_http_info(tenant_id, agent_id, conversation_id, opts)

```ruby
begin
  # Get all messages for a cognitive agent conversation
  data, status_code, headers = api_instance.get_cognitive_agent_messages_async_with_http_info(tenant_id, agent_id, conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentMessageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentMessagesApi->get_cognitive_agent_messages_async_with_http_info: #{e}"
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
| **cognitive_agent_message_dto_collection_query_parameters** | [**CognitiveAgentMessageDtoCollectionQueryParameters**](CognitiveAgentMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CognitiveAgentMessageDtoListEnvelope**](CognitiveAgentMessageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_cognitive_agent_messages_count_async

> <Int32Envelope> get_cognitive_agent_messages_count_async(tenant_id, agent_id, conversation_id, opts)

Get message count for a cognitive agent conversation

Returns the count of durable messages for the specified conversation, agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentMessagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
conversation_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_message_dto_collection_query_parameters: OpenapiClient::CognitiveAgentMessageDtoCollectionQueryParameters.new # CognitiveAgentMessageDtoCollectionQueryParameters | 
}

begin
  # Get message count for a cognitive agent conversation
  result = api_instance.get_cognitive_agent_messages_count_async(tenant_id, agent_id, conversation_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentMessagesApi->get_cognitive_agent_messages_count_async: #{e}"
end
```

#### Using the get_cognitive_agent_messages_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cognitive_agent_messages_count_async_with_http_info(tenant_id, agent_id, conversation_id, opts)

```ruby
begin
  # Get message count for a cognitive agent conversation
  data, status_code, headers = api_instance.get_cognitive_agent_messages_count_async_with_http_info(tenant_id, agent_id, conversation_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentMessagesApi->get_cognitive_agent_messages_count_async_with_http_info: #{e}"
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
| **cognitive_agent_message_dto_collection_query_parameters** | [**CognitiveAgentMessageDtoCollectionQueryParameters**](CognitiveAgentMessageDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

