# OpenapiClient::CognitiveSkillsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_cognitive_skill_async**](CognitiveSkillsApi.md#create_cognitive_skill_async) | **POST** /api/v2/IntelligenceService/CognitiveSkills | Create a new cognitive skill |
| [**delete_cognitive_skill_async**](CognitiveSkillsApi.md#delete_cognitive_skill_async) | **DELETE** /api/v2/IntelligenceService/CognitiveSkills/{id} | Delete a cognitive skill |
| [**get_cognitive_skill_by_id_async**](CognitiveSkillsApi.md#get_cognitive_skill_by_id_async) | **GET** /api/v2/IntelligenceService/CognitiveSkills/{id} | Get cognitive skill by ID |
| [**get_cognitive_skills_async**](CognitiveSkillsApi.md#get_cognitive_skills_async) | **GET** /api/v2/IntelligenceService/CognitiveSkills | Get all cognitive skills |
| [**get_cognitive_skills_count_async**](CognitiveSkillsApi.md#get_cognitive_skills_count_async) | **GET** /api/v2/IntelligenceService/CognitiveSkills/Count | Get cognitive skills count |
| [**update_cognitive_skill_async**](CognitiveSkillsApi.md#update_cognitive_skill_async) | **PUT** /api/v2/IntelligenceService/CognitiveSkills/{id} | Update a cognitive skill |


## create_cognitive_skill_async

> create_cognitive_skill_async(tenant_id, opts)

Create a new cognitive skill

Creates a new reusable cognitive skill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_skill_create_dto: OpenapiClient::CognitiveSkillCreateDto.new({name: 'name_example'}) # CognitiveSkillCreateDto | 
}

begin
  # Create a new cognitive skill
  api_instance.create_cognitive_skill_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->create_cognitive_skill_async: #{e}"
end
```

#### Using the create_cognitive_skill_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_cognitive_skill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new cognitive skill
  data, status_code, headers = api_instance.create_cognitive_skill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->create_cognitive_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_skill_create_dto** | [**CognitiveSkillCreateDto**](CognitiveSkillCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_cognitive_skill_async

> delete_cognitive_skill_async(tenant_id, id, opts)

Delete a cognitive skill

Deletes a reusable cognitive skill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a cognitive skill
  api_instance.delete_cognitive_skill_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->delete_cognitive_skill_async: #{e}"
end
```

#### Using the delete_cognitive_skill_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_cognitive_skill_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a cognitive skill
  data, status_code, headers = api_instance.delete_cognitive_skill_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->delete_cognitive_skill_async_with_http_info: #{e}"
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


## get_cognitive_skill_by_id_async

> <CognitiveSkillDtoEnvelope> get_cognitive_skill_by_id_async(tenant_id, id, opts)

Get cognitive skill by ID

Retrieves a specific reusable cognitive skill by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get cognitive skill by ID
  result = api_instance.get_cognitive_skill_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->get_cognitive_skill_by_id_async: #{e}"
end
```

#### Using the get_cognitive_skill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveSkillDtoEnvelope>, Integer, Hash)> get_cognitive_skill_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get cognitive skill by ID
  data, status_code, headers = api_instance.get_cognitive_skill_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveSkillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->get_cognitive_skill_by_id_async_with_http_info: #{e}"
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

[**CognitiveSkillDtoEnvelope**](CognitiveSkillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cognitive_skills_async

> <CognitiveSkillDtoListEnvelope> get_cognitive_skills_async(tenant_id, opts)

Get all cognitive skills

Retrieves all reusable cognitive skills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_skill_dto_collection_query_parameters: OpenapiClient::CognitiveSkillDtoCollectionQueryParameters.new # CognitiveSkillDtoCollectionQueryParameters | 
}

begin
  # Get all cognitive skills
  result = api_instance.get_cognitive_skills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->get_cognitive_skills_async: #{e}"
end
```

#### Using the get_cognitive_skills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CognitiveSkillDtoListEnvelope>, Integer, Hash)> get_cognitive_skills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all cognitive skills
  data, status_code, headers = api_instance.get_cognitive_skills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CognitiveSkillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->get_cognitive_skills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_skill_dto_collection_query_parameters** | [**CognitiveSkillDtoCollectionQueryParameters**](CognitiveSkillDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CognitiveSkillDtoListEnvelope**](CognitiveSkillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_cognitive_skills_count_async

> <Int32Envelope> get_cognitive_skills_count_async(tenant_id, opts)

Get cognitive skills count

Returns the count of reusable cognitive skills for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_skill_dto_collection_query_parameters: OpenapiClient::CognitiveSkillDtoCollectionQueryParameters.new # CognitiveSkillDtoCollectionQueryParameters | 
}

begin
  # Get cognitive skills count
  result = api_instance.get_cognitive_skills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->get_cognitive_skills_count_async: #{e}"
end
```

#### Using the get_cognitive_skills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_cognitive_skills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get cognitive skills count
  data, status_code, headers = api_instance.get_cognitive_skills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->get_cognitive_skills_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_skill_dto_collection_query_parameters** | [**CognitiveSkillDtoCollectionQueryParameters**](CognitiveSkillDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_cognitive_skill_async

> update_cognitive_skill_async(tenant_id, id, opts)

Update a cognitive skill

Updates an existing reusable cognitive skill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CognitiveSkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  cognitive_skill_update_dto: OpenapiClient::CognitiveSkillUpdateDto.new # CognitiveSkillUpdateDto | 
}

begin
  # Update a cognitive skill
  api_instance.update_cognitive_skill_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->update_cognitive_skill_async: #{e}"
end
```

#### Using the update_cognitive_skill_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_cognitive_skill_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a cognitive skill
  data, status_code, headers = api_instance.update_cognitive_skill_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CognitiveSkillsApi->update_cognitive_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **cognitive_skill_update_dto** | [**CognitiveSkillUpdateDto**](CognitiveSkillUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

