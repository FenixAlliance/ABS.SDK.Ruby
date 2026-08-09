# OpenapiClient::CognitiveAgentSkillsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_cognitive_agent_skill_async**](CognitiveAgentSkillsApi.md#create_cognitive_agent_skill_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills | Assign a skill to a cognitive agent |
| [**delete_cognitive_agent_skill_async**](CognitiveAgentSkillsApi.md#delete_cognitive_agent_skill_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/{id} | Remove a skill assignment from a cognitive agent |
| [**get_cognitive_agent_skill_by_id_async**](CognitiveAgentSkillsApi.md#get_cognitive_agent_skill_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/{id} | Get a cognitive agent skill assignment by ID |
| [**get_cognitive_agent_skills_async**](CognitiveAgentSkillsApi.md#get_cognitive_agent_skills_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills | Get all skill assignments for a cognitive agent |
| [**get_cognitive_agent_skills_count_async**](CognitiveAgentSkillsApi.md#get_cognitive_agent_skills_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/Count | Get skill assignment count for a cognitive agent |
| [**update_cognitive_agent_skill_async**](CognitiveAgentSkillsApi.md#update_cognitive_agent_skill_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Skills/{id} | Update a cognitive agent skill assignment |


## create_cognitive_agent_skill_async

> create_cognitive_agent_skill_async(tenant_id, agent_id, opts)

Assign a skill to a cognitive agent

Assigns a reusable catalog skill to the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_skill_create_dto: OpenapiClient::CognitiveAgentSkillCreateDto.new({cognitive_skill_id: 'cognitive_skill_id_example'}) # CognitiveAgentSkillCreateDto | 
}

begin
  # Assign a skill to a cognitive agent
  api_instance.create_cognitive_agent_skill_async(tenant_id, agent_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->create_cognitive_agent_skill_async: #{e}"
end
```

#### Using the create_cognitive_agent_skill_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_cognitive_agent_skill_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Assign a skill to a cognitive agent
  data, status_code, headers = api_instance.create_cognitive_agent_skill_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->create_cognitive_agent_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_skill_create_dto** | [**CognitiveAgentSkillCreateDto**](CognitiveAgentSkillCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_cognitive_agent_skill_async

> delete_cognitive_agent_skill_async(tenant_id, agent_id, id, opts)

Remove a skill assignment from a cognitive agent

Removes a skill assignment from the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a skill assignment from a cognitive agent
  api_instance.delete_cognitive_agent_skill_async(tenant_id, agent_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->delete_cognitive_agent_skill_async: #{e}"
end
```

#### Using the delete_cognitive_agent_skill_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_cognitive_agent_skill_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Remove a skill assignment from a cognitive agent
  data, status_code, headers = api_instance.delete_cognitive_agent_skill_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->delete_cognitive_agent_skill_async_with_http_info: #{e}"
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


## get_cognitive_agent_skill_by_id_async

> <CognitiveAgentSkillDtoEnvelope> get_cognitive_agent_skill_by_id_async(tenant_id, agent_id, id, opts)

Get a cognitive agent skill assignment by ID

Retrieves a specific skill assignment of a cognitive agent by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cognitive agent skill assignment by ID
  result = api_instance.get_cognitive_agent_skill_by_id_async(tenant_id, agent_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->get_cognitive_agent_skill_by_id_async: #{e}"
end
```

#### Using the get_cognitive_agent_skill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentSkillDtoEnvelope>, Integer, Hash)> get_cognitive_agent_skill_by_id_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Get a cognitive agent skill assignment by ID
  data, status_code, headers = api_instance.get_cognitive_agent_skill_by_id_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentSkillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->get_cognitive_agent_skill_by_id_async_with_http_info: #{e}"
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

[**CognitiveAgentSkillDtoEnvelope**](CognitiveAgentSkillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_agent_skills_async

> <CognitiveAgentSkillDtoListEnvelope> get_cognitive_agent_skills_async(tenant_id, agent_id, opts)

Get all skill assignments for a cognitive agent

Retrieves all skill assignments for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_skill_dto_collection_query_parameters: OpenapiClient::CognitiveAgentSkillDtoCollectionQueryParameters.new # CognitiveAgentSkillDtoCollectionQueryParameters | 
}

begin
  # Get all skill assignments for a cognitive agent
  result = api_instance.get_cognitive_agent_skills_async(tenant_id, agent_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->get_cognitive_agent_skills_async: #{e}"
end
```

#### Using the get_cognitive_agent_skills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentSkillDtoListEnvelope>, Integer, Hash)> get_cognitive_agent_skills_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Get all skill assignments for a cognitive agent
  data, status_code, headers = api_instance.get_cognitive_agent_skills_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentSkillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->get_cognitive_agent_skills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_skill_dto_collection_query_parameters** | [**CognitiveAgentSkillDtoCollectionQueryParameters**](CognitiveAgentSkillDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CognitiveAgentSkillDtoListEnvelope**](CognitiveAgentSkillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_cognitive_agent_skills_count_async

> <Int32Envelope> get_cognitive_agent_skills_count_async(tenant_id, agent_id, opts)

Get skill assignment count for a cognitive agent

Returns the count of skill assignments for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_skill_dto_collection_query_parameters: OpenapiClient::CognitiveAgentSkillDtoCollectionQueryParameters.new # CognitiveAgentSkillDtoCollectionQueryParameters | 
}

begin
  # Get skill assignment count for a cognitive agent
  result = api_instance.get_cognitive_agent_skills_count_async(tenant_id, agent_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->get_cognitive_agent_skills_count_async: #{e}"
end
```

#### Using the get_cognitive_agent_skills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cognitive_agent_skills_count_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Get skill assignment count for a cognitive agent
  data, status_code, headers = api_instance.get_cognitive_agent_skills_count_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->get_cognitive_agent_skills_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_skill_dto_collection_query_parameters** | [**CognitiveAgentSkillDtoCollectionQueryParameters**](CognitiveAgentSkillDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cognitive_agent_skill_async

> update_cognitive_agent_skill_async(tenant_id, agent_id, id, opts)

Update a cognitive agent skill assignment

Updates the per-assignment overrides of a skill assignment for the specified agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_skill_update_dto: OpenapiClient::CognitiveAgentSkillUpdateDto.new # CognitiveAgentSkillUpdateDto | 
}

begin
  # Update a cognitive agent skill assignment
  api_instance.update_cognitive_agent_skill_async(tenant_id, agent_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->update_cognitive_agent_skill_async: #{e}"
end
```

#### Using the update_cognitive_agent_skill_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_cognitive_agent_skill_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Update a cognitive agent skill assignment
  data, status_code, headers = api_instance.update_cognitive_agent_skill_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentSkillsApi->update_cognitive_agent_skill_async_with_http_info: #{e}"
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
| **cognitive_agent_skill_update_dto** | [**CognitiveAgentSkillUpdateDto**](CognitiveAgentSkillUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

