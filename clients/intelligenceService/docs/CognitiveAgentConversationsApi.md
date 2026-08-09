# OpenapiClient::CognitiveAgentConversationsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_cognitive_agent_conversation_async**](CognitiveAgentConversationsApi.md#create_cognitive_agent_conversation_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations | Create a new cognitive agent conversation |
| [**delete_cognitive_agent_conversation_async**](CognitiveAgentConversationsApi.md#delete_cognitive_agent_conversation_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{id} | Delete a cognitive agent conversation |
| [**get_cognitive_agent_conversation_by_id_async**](CognitiveAgentConversationsApi.md#get_cognitive_agent_conversation_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{id} | Get a cognitive agent conversation by ID |
| [**get_cognitive_agent_conversations_async**](CognitiveAgentConversationsApi.md#get_cognitive_agent_conversations_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations | Get all conversations for a cognitive agent |
| [**get_cognitive_agent_conversations_count_async**](CognitiveAgentConversationsApi.md#get_cognitive_agent_conversations_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/Count | Get conversation count for a cognitive agent |
| [**update_cognitive_agent_conversation_async**](CognitiveAgentConversationsApi.md#update_cognitive_agent_conversation_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Conversations/{id} | Update a cognitive agent conversation |


## create_cognitive_agent_conversation_async

> create_cognitive_agent_conversation_async(tenant_id, agent_id, opts)

Create a new cognitive agent conversation

Creates a new managed conversation for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_conversation_create_dto: OpenapiClient::CognitiveAgentConversationCreateDto.new # CognitiveAgentConversationCreateDto | 
}

begin
  # Create a new cognitive agent conversation
  api_instance.create_cognitive_agent_conversation_async(tenant_id, agent_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->create_cognitive_agent_conversation_async: #{e}"
end
```

#### Using the create_cognitive_agent_conversation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_cognitive_agent_conversation_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Create a new cognitive agent conversation
  data, status_code, headers = api_instance.create_cognitive_agent_conversation_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->create_cognitive_agent_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_conversation_create_dto** | [**CognitiveAgentConversationCreateDto**](CognitiveAgentConversationCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_cognitive_agent_conversation_async

> delete_cognitive_agent_conversation_async(tenant_id, agent_id, id, opts)

Delete a cognitive agent conversation

Deletes a managed conversation for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a cognitive agent conversation
  api_instance.delete_cognitive_agent_conversation_async(tenant_id, agent_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->delete_cognitive_agent_conversation_async: #{e}"
end
```

#### Using the delete_cognitive_agent_conversation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_cognitive_agent_conversation_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Delete a cognitive agent conversation
  data, status_code, headers = api_instance.delete_cognitive_agent_conversation_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->delete_cognitive_agent_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_agent_conversation_by_id_async

> <CognitiveAgentConversationDtoEnvelope> get_cognitive_agent_conversation_by_id_async(tenant_id, agent_id, id, opts)

Get a cognitive agent conversation by ID

Retrieves a specific managed conversation of a cognitive agent by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cognitive agent conversation by ID
  result = api_instance.get_cognitive_agent_conversation_by_id_async(tenant_id, agent_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->get_cognitive_agent_conversation_by_id_async: #{e}"
end
```

#### Using the get_cognitive_agent_conversation_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentConversationDtoEnvelope>, Integer, Hash)> get_cognitive_agent_conversation_by_id_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Get a cognitive agent conversation by ID
  data, status_code, headers = api_instance.get_cognitive_agent_conversation_by_id_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentConversationDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->get_cognitive_agent_conversation_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CognitiveAgentConversationDtoEnvelope**](CognitiveAgentConversationDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_agent_conversations_async

> <CognitiveAgentConversationDtoListEnvelope> get_cognitive_agent_conversations_async(tenant_id, agent_id, opts)

Get all conversations for a cognitive agent

Retrieves all managed conversations for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_conversation_dto_collection_query_parameters: OpenapiClient::CognitiveAgentConversationDtoCollectionQueryParameters.new # CognitiveAgentConversationDtoCollectionQueryParameters | 
}

begin
  # Get all conversations for a cognitive agent
  result = api_instance.get_cognitive_agent_conversations_async(tenant_id, agent_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->get_cognitive_agent_conversations_async: #{e}"
end
```

#### Using the get_cognitive_agent_conversations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentConversationDtoListEnvelope>, Integer, Hash)> get_cognitive_agent_conversations_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Get all conversations for a cognitive agent
  data, status_code, headers = api_instance.get_cognitive_agent_conversations_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentConversationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->get_cognitive_agent_conversations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_conversation_dto_collection_query_parameters** | [**CognitiveAgentConversationDtoCollectionQueryParameters**](CognitiveAgentConversationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CognitiveAgentConversationDtoListEnvelope**](CognitiveAgentConversationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_cognitive_agent_conversations_count_async

> <Int32Envelope> get_cognitive_agent_conversations_count_async(tenant_id, agent_id, opts)

Get conversation count for a cognitive agent

Returns the count of managed conversations for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_conversation_dto_collection_query_parameters: OpenapiClient::CognitiveAgentConversationDtoCollectionQueryParameters.new # CognitiveAgentConversationDtoCollectionQueryParameters | 
}

begin
  # Get conversation count for a cognitive agent
  result = api_instance.get_cognitive_agent_conversations_count_async(tenant_id, agent_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->get_cognitive_agent_conversations_count_async: #{e}"
end
```

#### Using the get_cognitive_agent_conversations_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cognitive_agent_conversations_count_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Get conversation count for a cognitive agent
  data, status_code, headers = api_instance.get_cognitive_agent_conversations_count_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->get_cognitive_agent_conversations_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_conversation_dto_collection_query_parameters** | [**CognitiveAgentConversationDtoCollectionQueryParameters**](CognitiveAgentConversationDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cognitive_agent_conversation_async

> update_cognitive_agent_conversation_async(tenant_id, agent_id, id, opts)

Update a cognitive agent conversation

Updates an existing managed conversation for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentConversationsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_conversation_update_dto: OpenapiClient::CognitiveAgentConversationUpdateDto.new # CognitiveAgentConversationUpdateDto | 
}

begin
  # Update a cognitive agent conversation
  api_instance.update_cognitive_agent_conversation_async(tenant_id, agent_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->update_cognitive_agent_conversation_async: #{e}"
end
```

#### Using the update_cognitive_agent_conversation_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_cognitive_agent_conversation_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Update a cognitive agent conversation
  data, status_code, headers = api_instance.update_cognitive_agent_conversation_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentConversationsApi->update_cognitive_agent_conversation_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_conversation_update_dto** | [**CognitiveAgentConversationUpdateDto**](CognitiveAgentConversationUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

