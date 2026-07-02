# OpenapiClient::SkillsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_skill_async**](SkillsApi.md#create_skill_async) | **POST** /api/v2/SocialService/Skills | Create a skill |
| [**delete_skill_async**](SkillsApi.md#delete_skill_async) | **DELETE** /api/v2/SocialService/Skills/{skillId} | Delete a skill |
| [**get_skill_by_id_async**](SkillsApi.md#get_skill_by_id_async) | **GET** /api/v2/SocialService/Skills/{skillId} | Get skill by ID |
| [**get_skills_async**](SkillsApi.md#get_skills_async) | **GET** /api/v2/SocialService/Skills | Get skills |
| [**get_skills_count_async**](SkillsApi.md#get_skills_count_async) | **GET** /api/v2/SocialService/Skills/Count | Count skills |
| [**patch_skill_async**](SkillsApi.md#patch_skill_async) | **PATCH** /api/v2/SocialService/Skills/{skillId} | Patch a skill |
| [**update_skill_async**](SkillsApi.md#update_skill_async) | **PUT** /api/v2/SocialService/Skills/{skillId} | Update a skill |


## create_skill_async

> <EmptyEnvelope> create_skill_async(tenant_id, opts)

Create a skill

Creates a new skill catalog entry for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  skill_create_dto: OpenapiClient::SkillCreateDto.new({name: 'name_example'}) # SkillCreateDto | 
}

begin
  # Create a skill
  result = api_instance.create_skill_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->create_skill_async: #{e}"
end
```

#### Using the create_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_skill_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a skill
  data, status_code, headers = api_instance.create_skill_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->create_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **skill_create_dto** | [**SkillCreateDto**](SkillCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_skill_async

> <EmptyEnvelope> delete_skill_async(tenant_id, skill_id, opts)

Delete a skill

Deletes a skill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a skill
  result = api_instance.delete_skill_async(tenant_id, skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->delete_skill_async: #{e}"
end
```

#### Using the delete_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_skill_async_with_http_info(tenant_id, skill_id, opts)

```ruby
begin
  # Delete a skill
  data, status_code, headers = api_instance.delete_skill_async_with_http_info(tenant_id, skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->delete_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_skill_by_id_async

> <SkillDtoEnvelope> get_skill_by_id_async(tenant_id, skill_id, opts)

Get skill by ID

Retrieves a specific skill by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get skill by ID
  result = api_instance.get_skill_by_id_async(tenant_id, skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->get_skill_by_id_async: #{e}"
end
```

#### Using the get_skill_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SkillDtoEnvelope>, Integer, Hash)> get_skill_by_id_async_with_http_info(tenant_id, skill_id, opts)

```ruby
begin
  # Get skill by ID
  data, status_code, headers = api_instance.get_skill_by_id_async_with_http_info(tenant_id, skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SkillDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->get_skill_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SkillDtoEnvelope**](SkillDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_skills_async

> <SkillDtoListEnvelope> get_skills_async(tenant_id, opts)

Get skills

Retrieves the skill catalog for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get skills
  result = api_instance.get_skills_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->get_skills_async: #{e}"
end
```

#### Using the get_skills_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SkillDtoListEnvelope>, Integer, Hash)> get_skills_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get skills
  data, status_code, headers = api_instance.get_skills_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SkillDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->get_skills_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SkillDtoListEnvelope**](SkillDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_skills_count_async

> <Int32Envelope> get_skills_count_async(tenant_id, opts)

Count skills

Counts skill catalog entries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count skills
  result = api_instance.get_skills_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->get_skills_count_async: #{e}"
end
```

#### Using the get_skills_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_skills_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count skills
  data, status_code, headers = api_instance.get_skills_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->get_skills_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_skill_async

> <EmptyEnvelope> patch_skill_async(tenant_id, skill_id, opts)

Patch a skill

Partially updates an existing skill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a skill
  result = api_instance.patch_skill_async(tenant_id, skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->patch_skill_async: #{e}"
end
```

#### Using the patch_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_skill_async_with_http_info(tenant_id, skill_id, opts)

```ruby
begin
  # Patch a skill
  data, status_code, headers = api_instance.patch_skill_async_with_http_info(tenant_id, skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->patch_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_skill_async

> <EmptyEnvelope> update_skill_async(tenant_id, skill_id, opts)

Update a skill

Updates an existing skill for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SkillsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
skill_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  skill_update_dto: OpenapiClient::SkillUpdateDto.new # SkillUpdateDto | 
}

begin
  # Update a skill
  result = api_instance.update_skill_async(tenant_id, skill_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->update_skill_async: #{e}"
end
```

#### Using the update_skill_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_skill_async_with_http_info(tenant_id, skill_id, opts)

```ruby
begin
  # Update a skill
  data, status_code, headers = api_instance.update_skill_async_with_http_info(tenant_id, skill_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SkillsApi->update_skill_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **skill_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **skill_update_dto** | [**SkillUpdateDto**](SkillUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

