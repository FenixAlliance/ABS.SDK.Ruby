# OpenapiClient::CognitiveAgentVariablesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_cognitive_agent_variable_async**](CognitiveAgentVariablesApi.md#create_cognitive_agent_variable_async) | **POST** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables | Add a variable to a cognitive agent |
| [**delete_cognitive_agent_variable_async**](CognitiveAgentVariablesApi.md#delete_cognitive_agent_variable_async) | **DELETE** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/{id} | Remove a variable from a cognitive agent |
| [**get_cognitive_agent_variable_by_id_async**](CognitiveAgentVariablesApi.md#get_cognitive_agent_variable_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/{id} | Get a cognitive agent variable by ID |
| [**get_cognitive_agent_variables_async**](CognitiveAgentVariablesApi.md#get_cognitive_agent_variables_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables | Get all variables for a cognitive agent |
| [**get_cognitive_agent_variables_count_async**](CognitiveAgentVariablesApi.md#get_cognitive_agent_variables_count_async) | **GET** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/Count | Get variable count for a cognitive agent |
| [**update_cognitive_agent_variable_async**](CognitiveAgentVariablesApi.md#update_cognitive_agent_variable_async) | **PUT** /api/v2/IntelligenceService/CognitiveAgents/{agentId}/Variables/{id} | Update a cognitive agent variable |


## create_cognitive_agent_variable_async

> create_cognitive_agent_variable_async(tenant_id, agent_id, opts)

Add a variable to a cognitive agent

Adds a key/value variable to the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentVariablesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_variable_create_dto: OpenapiClient::CognitiveAgentVariableCreateDto.new({key: 'key_example'}) # CognitiveAgentVariableCreateDto | 
}

begin
  # Add a variable to a cognitive agent
  api_instance.create_cognitive_agent_variable_async(tenant_id, agent_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->create_cognitive_agent_variable_async: #{e}"
end
```

#### Using the create_cognitive_agent_variable_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_cognitive_agent_variable_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Add a variable to a cognitive agent
  data, status_code, headers = api_instance.create_cognitive_agent_variable_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->create_cognitive_agent_variable_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_variable_create_dto** | [**CognitiveAgentVariableCreateDto**](CognitiveAgentVariableCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_cognitive_agent_variable_async

> delete_cognitive_agent_variable_async(tenant_id, agent_id, id, opts)

Remove a variable from a cognitive agent

Removes a variable from the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentVariablesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove a variable from a cognitive agent
  api_instance.delete_cognitive_agent_variable_async(tenant_id, agent_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->delete_cognitive_agent_variable_async: #{e}"
end
```

#### Using the delete_cognitive_agent_variable_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_cognitive_agent_variable_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Remove a variable from a cognitive agent
  data, status_code, headers = api_instance.delete_cognitive_agent_variable_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->delete_cognitive_agent_variable_async_with_http_info: #{e}"
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


## get_cognitive_agent_variable_by_id_async

> <CognitiveAgentVariableDtoEnvelope> get_cognitive_agent_variable_by_id_async(tenant_id, agent_id, id, opts)

Get a cognitive agent variable by ID

Retrieves a specific variable of a cognitive agent by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentVariablesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a cognitive agent variable by ID
  result = api_instance.get_cognitive_agent_variable_by_id_async(tenant_id, agent_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->get_cognitive_agent_variable_by_id_async: #{e}"
end
```

#### Using the get_cognitive_agent_variable_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentVariableDtoEnvelope>, Integer, Hash)> get_cognitive_agent_variable_by_id_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Get a cognitive agent variable by ID
  data, status_code, headers = api_instance.get_cognitive_agent_variable_by_id_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentVariableDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->get_cognitive_agent_variable_by_id_async_with_http_info: #{e}"
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

[**CognitiveAgentVariableDtoEnvelope**](CognitiveAgentVariableDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_agent_variables_async

> <CognitiveAgentVariableDtoListEnvelope> get_cognitive_agent_variables_async(tenant_id, agent_id, opts)

Get all variables for a cognitive agent

Retrieves all key/value variables for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentVariablesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_variable_dto_collection_query_parameters: OpenapiClient::CognitiveAgentVariableDtoCollectionQueryParameters.new # CognitiveAgentVariableDtoCollectionQueryParameters | 
}

begin
  # Get all variables for a cognitive agent
  result = api_instance.get_cognitive_agent_variables_async(tenant_id, agent_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->get_cognitive_agent_variables_async: #{e}"
end
```

#### Using the get_cognitive_agent_variables_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveAgentVariableDtoListEnvelope>, Integer, Hash)> get_cognitive_agent_variables_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Get all variables for a cognitive agent
  data, status_code, headers = api_instance.get_cognitive_agent_variables_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveAgentVariableDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->get_cognitive_agent_variables_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_variable_dto_collection_query_parameters** | [**CognitiveAgentVariableDtoCollectionQueryParameters**](CognitiveAgentVariableDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CognitiveAgentVariableDtoListEnvelope**](CognitiveAgentVariableDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_cognitive_agent_variables_count_async

> <Int32Envelope> get_cognitive_agent_variables_count_async(tenant_id, agent_id, opts)

Get variable count for a cognitive agent

Returns the count of variables for the specified cognitive agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentVariablesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_variable_dto_collection_query_parameters: OpenapiClient::CognitiveAgentVariableDtoCollectionQueryParameters.new # CognitiveAgentVariableDtoCollectionQueryParameters | 
}

begin
  # Get variable count for a cognitive agent
  result = api_instance.get_cognitive_agent_variables_count_async(tenant_id, agent_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->get_cognitive_agent_variables_count_async: #{e}"
end
```

#### Using the get_cognitive_agent_variables_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cognitive_agent_variables_count_async_with_http_info(tenant_id, agent_id, opts)

```ruby
begin
  # Get variable count for a cognitive agent
  data, status_code, headers = api_instance.get_cognitive_agent_variables_count_async_with_http_info(tenant_id, agent_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->get_cognitive_agent_variables_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **agent_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_agent_variable_dto_collection_query_parameters** | [**CognitiveAgentVariableDtoCollectionQueryParameters**](CognitiveAgentVariableDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cognitive_agent_variable_async

> update_cognitive_agent_variable_async(tenant_id, agent_id, id, opts)

Update a cognitive agent variable

Updates the value of a variable for the specified agent and tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveAgentVariablesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
agent_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_agent_variable_update_dto: OpenapiClient::CognitiveAgentVariableUpdateDto.new # CognitiveAgentVariableUpdateDto | 
}

begin
  # Update a cognitive agent variable
  api_instance.update_cognitive_agent_variable_async(tenant_id, agent_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->update_cognitive_agent_variable_async: #{e}"
end
```

#### Using the update_cognitive_agent_variable_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_cognitive_agent_variable_async_with_http_info(tenant_id, agent_id, id, opts)

```ruby
begin
  # Update a cognitive agent variable
  data, status_code, headers = api_instance.update_cognitive_agent_variable_async_with_http_info(tenant_id, agent_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveAgentVariablesApi->update_cognitive_agent_variable_async_with_http_info: #{e}"
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
| **cognitive_agent_variable_update_dto** | [**CognitiveAgentVariableUpdateDto**](CognitiveAgentVariableUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

