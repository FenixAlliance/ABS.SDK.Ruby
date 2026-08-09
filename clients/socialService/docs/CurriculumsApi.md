# OpenapiClient::CurriculumsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_curriculum_async**](CurriculumsApi.md#create_curriculum_async) | **POST** /api/v2/SocialService/Curriculums | Create a curriculum |
| [**delete_curriculum_async**](CurriculumsApi.md#delete_curriculum_async) | **DELETE** /api/v2/SocialService/Curriculums/{curriculumId} | Delete a curriculum |
| [**get_curriculum_async**](CurriculumsApi.md#get_curriculum_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId} | Get curriculum by ID |
| [**get_curriculums_async**](CurriculumsApi.md#get_curriculums_async) | **GET** /api/v2/SocialService/Curriculums | Get curricula |
| [**get_curriculums_count_async**](CurriculumsApi.md#get_curriculums_count_async) | **GET** /api/v2/SocialService/Curriculums/Count | Count curricula |
| [**patch_curriculum_async**](CurriculumsApi.md#patch_curriculum_async) | **PATCH** /api/v2/SocialService/Curriculums/{curriculumId} | Patch a curriculum |
| [**update_curriculum_async**](CurriculumsApi.md#update_curriculum_async) | **PUT** /api/v2/SocialService/Curriculums/{curriculumId} | Update a curriculum |


## create_curriculum_async

> <EmptyEnvelope> create_curriculum_async(social_profile_id, opts)

Create a curriculum

Creates a curriculum (CV) on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_create_dto: OpenapiClient::CurriculumCreateDto.new # CurriculumCreateDto | 
}

begin
  # Create a curriculum
  result = api_instance.create_curriculum_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->create_curriculum_async: #{e}"
end
```

#### Using the create_curriculum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_curriculum_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Create a curriculum
  data, status_code, headers = api_instance.create_curriculum_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->create_curriculum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_create_dto** | [**CurriculumCreateDto**](CurriculumCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_curriculum_async

> <EmptyEnvelope> delete_curriculum_async(social_profile_id, curriculum_id, opts)

Delete a curriculum

Deletes a curriculum authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a curriculum
  result = api_instance.delete_curriculum_async(social_profile_id, curriculum_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->delete_curriculum_async: #{e}"
end
```

#### Using the delete_curriculum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)

```ruby
begin
  # Delete a curriculum
  data, status_code, headers = api_instance.delete_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->delete_curriculum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **curriculum_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_curriculum_async

> <CurriculumDtoEnvelope> get_curriculum_async(social_profile_id, curriculum_id, opts)

Get curriculum by ID

Retrieves a specific curriculum authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get curriculum by ID
  result = api_instance.get_curriculum_async(social_profile_id, curriculum_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->get_curriculum_async: #{e}"
end
```

#### Using the get_curriculum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurriculumDtoEnvelope>, Integer, Hash)> get_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)

```ruby
begin
  # Get curriculum by ID
  data, status_code, headers = api_instance.get_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurriculumDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->get_curriculum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **curriculum_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CurriculumDtoEnvelope**](CurriculumDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_curriculums_async

> <CurriculumDtoListEnvelope> get_curriculums_async(social_profile_id, opts)

Get curricula

Retrieves the curricula (CVs) authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_dto_collection_query_parameters: OpenapiClient::CurriculumDtoCollectionQueryParameters.new # CurriculumDtoCollectionQueryParameters | 
}

begin
  # Get curricula
  result = api_instance.get_curriculums_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->get_curriculums_async: #{e}"
end
```

#### Using the get_curriculums_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurriculumDtoListEnvelope>, Integer, Hash)> get_curriculums_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Get curricula
  data, status_code, headers = api_instance.get_curriculums_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurriculumDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->get_curriculums_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_dto_collection_query_parameters** | [**CurriculumDtoCollectionQueryParameters**](CurriculumDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CurriculumDtoListEnvelope**](CurriculumDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_curriculums_count_async

> <Int32Envelope> get_curriculums_count_async(social_profile_id, opts)

Count curricula

Returns the count of curricula authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_dto_collection_query_parameters: OpenapiClient::CurriculumDtoCollectionQueryParameters.new # CurriculumDtoCollectionQueryParameters | 
}

begin
  # Count curricula
  result = api_instance.get_curriculums_count_async(social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->get_curriculums_count_async: #{e}"
end
```

#### Using the get_curriculums_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_curriculums_count_async_with_http_info(social_profile_id, opts)

```ruby
begin
  # Count curricula
  data, status_code, headers = api_instance.get_curriculums_count_async_with_http_info(social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->get_curriculums_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_dto_collection_query_parameters** | [**CurriculumDtoCollectionQueryParameters**](CurriculumDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_curriculum_async

> <EmptyEnvelope> patch_curriculum_async(social_profile_id, curriculum_id, opts)

Patch a curriculum

Partially updates an existing curriculum authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a curriculum
  result = api_instance.patch_curriculum_async(social_profile_id, curriculum_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->patch_curriculum_async: #{e}"
end
```

#### Using the patch_curriculum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)

```ruby
begin
  # Patch a curriculum
  data, status_code, headers = api_instance.patch_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->patch_curriculum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **curriculum_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_curriculum_async

> <EmptyEnvelope> update_curriculum_async(social_profile_id, curriculum_id, opts)

Update a curriculum

Updates an existing curriculum authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumsApi.new
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_update_dto: OpenapiClient::CurriculumUpdateDto.new # CurriculumUpdateDto | 
}

begin
  # Update a curriculum
  result = api_instance.update_curriculum_async(social_profile_id, curriculum_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->update_curriculum_async: #{e}"
end
```

#### Using the update_curriculum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)

```ruby
begin
  # Update a curriculum
  data, status_code, headers = api_instance.update_curriculum_async_with_http_info(social_profile_id, curriculum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumsApi->update_curriculum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **social_profile_id** | **String** |  |  |
| **curriculum_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_update_dto** | [**CurriculumUpdateDto**](CurriculumUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

