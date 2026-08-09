# OpenapiClient::CognitiveAgentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_cognitive_agent_async**](CognitiveAgentsApi.md#create_cognitive_agent_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents | Create a new cognitive agent |
| [**delete_cognitive_agent_async**](CognitiveAgentsApi.md#delete_cognitive_agent_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{id} | Delete a cognitive agent |
| [**get_cognitive_agent_by_id_async**](CognitiveAgentsApi.md#get_cognitive_agent_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{id} | Get cognitive agent by ID |
| [**get_cognitive_agents_async**](CognitiveAgentsApi.md#get_cognitive_agents_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents | Get all cognitive agents |
| [**get_cognitive_agents_count_async**](CognitiveAgentsApi.md#get_cognitive_agents_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/Count | Get cognitive agents count |
| [**update_cognitive_agent_async**](CognitiveAgentsApi.md#update_cognitive_agent_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{id} | Update a cognitive agent |


## create_cognitive_agent_async

> create_cognitive_agent_async(tenant_id, opts)

Create a new cognitive agent

Creates a new managed cognitive agent for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_create_dto: OpenapiClient::CognitiveAgentCreateDto.new({name: 'name_example'}) # CognitiveAgentCreateDto | 
}

begin
  # Create a new cognitive agent
  api_instance.create_cognitive_agent_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->create_cognitive_agent_async: #{e}"
end
```

#### Using the create_cognitive_agent_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_cognitive_agent_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new cognitive agent
  data, status_code, headers = api_instance.create_cognitive_agent_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->create_cognitive_agent_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_create_dto** | [**CognitiveAgentCreateDto**](CognitiveAgentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_cognitive_agent_async

> delete_cognitive_agent_async(tenant_id, id, opts)

Delete a cognitive agent

Deletes a managed cognitive agent for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a cognitive agent
  api_instance.delete_cognitive_agent_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->delete_cognitive_agent_async: #{e}"
end
```

#### Using the delete_cognitive_agent_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_cognitive_agent_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a cognitive agent
  data, status_code, headers = api_instance.delete_cognitive_agent_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->delete_cognitive_agent_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_cognitive_agent_by_id_async

> <CognitiveAgentDtoEnvelope> get_cognitive_agent_by_id_async(tenant_id, id, opts)

Get cognitive agent by ID

Retrieves a specific managed cognitive agent by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get cognitive agent by ID
  result = api_instance.get_cognitive_agent_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->get_cognitive_agent_by_id_async: #{e}"
end
```

#### Using the get_cognitive_agent_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentDtoEnvelope>, Integer, Hash)> get_cognitive_agent_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get cognitive agent by ID
  data, status_code, headers = api_instance.get_cognitive_agent_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->get_cognitive_agent_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CognitiveAgentDtoEnvelope**](CognitiveAgentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_agents_async

> <CognitiveAgentDtoListEnvelope> get_cognitive_agents_async(tenant_id, opts)

Get all cognitive agents

Retrieves all managed cognitive agents for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_dto_collection_query_parameters: OpenapiClient::CognitiveAgentDtoCollectionQueryParameters.new # CognitiveAgentDtoCollectionQueryParameters | 
}

begin
  # Get all cognitive agents
  result = api_instance.get_cognitive_agents_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->get_cognitive_agents_async: #{e}"
end
```

#### Using the get_cognitive_agents_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentDtoListEnvelope>, Integer, Hash)> get_cognitive_agents_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all cognitive agents
  data, status_code, headers = api_instance.get_cognitive_agents_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->get_cognitive_agents_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_dto_collection_query_parameters** | [**CognitiveAgentDtoCollectionQueryParameters**](CognitiveAgentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CognitiveAgentDtoListEnvelope**](CognitiveAgentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_cognitive_agents_count_async

> <Int32Envelope> get_cognitive_agents_count_async(tenant_id, opts)

Get cognitive agents count

Returns the count of managed cognitive agents for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_dto_collection_query_parameters: OpenapiClient::CognitiveAgentDtoCollectionQueryParameters.new # CognitiveAgentDtoCollectionQueryParameters | 
}

begin
  # Get cognitive agents count
  result = api_instance.get_cognitive_agents_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->get_cognitive_agents_count_async: #{e}"
end
```

#### Using the get_cognitive_agents_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cognitive_agents_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get cognitive agents count
  data, status_code, headers = api_instance.get_cognitive_agents_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->get_cognitive_agents_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_dto_collection_query_parameters** | [**CognitiveAgentDtoCollectionQueryParameters**](CognitiveAgentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cognitive_agent_async

> update_cognitive_agent_async(tenant_id, id, opts)

Update a cognitive agent

Updates an existing managed cognitive agent for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_update_dto: OpenapiClient::CognitiveAgentUpdateDto.new # CognitiveAgentUpdateDto | 
}

begin
  # Update a cognitive agent
  api_instance.update_cognitive_agent_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->update_cognitive_agent_async: #{e}"
end
```

#### Using the update_cognitive_agent_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_cognitive_agent_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a cognitive agent
  data, status_code, headers = api_instance.update_cognitive_agent_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentsApi->update_cognitive_agent_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_update_dto** | [**CognitiveAgentUpdateDto**](CognitiveAgentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

