# OpenapiClient::CurriculumExperiencesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_curriculum_experience_async**](CurriculumExperiencesApi.md#create_curriculum_experience_async) | **POST** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences | Create a curriculum experience |
| [**delete_curriculum_experience_async**](CurriculumExperiencesApi.md#delete_curriculum_experience_async) | **DELETE** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Delete a curriculum experience |
| [**get_curriculum_experience_async**](CurriculumExperiencesApi.md#get_curriculum_experience_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Get curriculum experience by ID |
| [**get_curriculum_experiences_async**](CurriculumExperiencesApi.md#get_curriculum_experiences_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences | Get curriculum experiences |
| [**get_curriculum_experiences_count_async**](CurriculumExperiencesApi.md#get_curriculum_experiences_count_async) | **GET** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/Count | Count curriculum experiences |
| [**patch_curriculum_experience_async**](CurriculumExperiencesApi.md#patch_curriculum_experience_async) | **PATCH** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Patch a curriculum experience |
| [**update_curriculum_experience_async**](CurriculumExperiencesApi.md#update_curriculum_experience_async) | **PUT** /api/v2/SocialService/Curriculums/{curriculumId}/Experiences/{experienceId} | Update a curriculum experience |


## create_curriculum_experience_async

> <EmptyEnvelope> create_curriculum_experience_async(curriculum_id, social_profile_id, opts)

Create a curriculum experience

Adds a work-experience record to a curriculum authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_experience_create_dto: OpenapiClient::CurriculumExperienceCreateDto.new # CurriculumExperienceCreateDto | 
}

begin
  # Create a curriculum experience
  result = api_instance.create_curriculum_experience_async(curriculum_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->create_curriculum_experience_async: #{e}"
end
```

#### Using the create_curriculum_experience_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_curriculum_experience_async_with_http_info(curriculum_id, social_profile_id, opts)

```ruby
begin
  # Create a curriculum experience
  data, status_code, headers = api_instance.create_curriculum_experience_async_with_http_info(curriculum_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->create_curriculum_experience_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_experience_create_dto** | [**CurriculumExperienceCreateDto**](CurriculumExperienceCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_curriculum_experience_async

> <EmptyEnvelope> delete_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)

Delete a curriculum experience

Removes a work-experience record from a curriculum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
experience_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a curriculum experience
  result = api_instance.delete_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->delete_curriculum_experience_async: #{e}"
end
```

#### Using the delete_curriculum_experience_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)

```ruby
begin
  # Delete a curriculum experience
  data, status_code, headers = api_instance.delete_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->delete_curriculum_experience_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **experience_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
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


## get_curriculum_experience_async

> <CurriculumExperienceDtoEnvelope> get_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)

Get curriculum experience by ID

Retrieves a specific work-experience record of a curriculum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
experience_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get curriculum experience by ID
  result = api_instance.get_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->get_curriculum_experience_async: #{e}"
end
```

#### Using the get_curriculum_experience_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurriculumExperienceDtoEnvelope>, Integer, Hash)> get_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)

```ruby
begin
  # Get curriculum experience by ID
  data, status_code, headers = api_instance.get_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurriculumExperienceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->get_curriculum_experience_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **experience_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CurriculumExperienceDtoEnvelope**](CurriculumExperienceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_curriculum_experiences_async

> <CurriculumExperienceDtoListEnvelope> get_curriculum_experiences_async(curriculum_id, social_profile_id, opts)

Get curriculum experiences

Retrieves the work-experience records of a curriculum authored on the specified social profile.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_experience_dto_collection_query_parameters: OpenapiClient::CurriculumExperienceDtoCollectionQueryParameters.new # CurriculumExperienceDtoCollectionQueryParameters | 
}

begin
  # Get curriculum experiences
  result = api_instance.get_curriculum_experiences_async(curriculum_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->get_curriculum_experiences_async: #{e}"
end
```

#### Using the get_curriculum_experiences_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurriculumExperienceDtoListEnvelope>, Integer, Hash)> get_curriculum_experiences_async_with_http_info(curriculum_id, social_profile_id, opts)

```ruby
begin
  # Get curriculum experiences
  data, status_code, headers = api_instance.get_curriculum_experiences_async_with_http_info(curriculum_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurriculumExperienceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->get_curriculum_experiences_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_experience_dto_collection_query_parameters** | [**CurriculumExperienceDtoCollectionQueryParameters**](CurriculumExperienceDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CurriculumExperienceDtoListEnvelope**](CurriculumExperienceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_curriculum_experiences_count_async

> <Int32Envelope> get_curriculum_experiences_count_async(curriculum_id, social_profile_id, opts)

Count curriculum experiences

Returns the count of work-experience records of a curriculum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_experience_dto_collection_query_parameters: OpenapiClient::CurriculumExperienceDtoCollectionQueryParameters.new # CurriculumExperienceDtoCollectionQueryParameters | 
}

begin
  # Count curriculum experiences
  result = api_instance.get_curriculum_experiences_count_async(curriculum_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->get_curriculum_experiences_count_async: #{e}"
end
```

#### Using the get_curriculum_experiences_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_curriculum_experiences_count_async_with_http_info(curriculum_id, social_profile_id, opts)

```ruby
begin
  # Count curriculum experiences
  data, status_code, headers = api_instance.get_curriculum_experiences_count_async_with_http_info(curriculum_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->get_curriculum_experiences_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_experience_dto_collection_query_parameters** | [**CurriculumExperienceDtoCollectionQueryParameters**](CurriculumExperienceDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_curriculum_experience_async

> <EmptyEnvelope> patch_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)

Patch a curriculum experience

Partially updates an existing work-experience record of a curriculum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
experience_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a curriculum experience
  result = api_instance.patch_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->patch_curriculum_experience_async: #{e}"
end
```

#### Using the patch_curriculum_experience_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)

```ruby
begin
  # Patch a curriculum experience
  data, status_code, headers = api_instance.patch_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->patch_curriculum_experience_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **experience_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
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


## update_curriculum_experience_async

> <EmptyEnvelope> update_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)

Update a curriculum experience

Updates an existing work-experience record of a curriculum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurriculumExperiencesApi.new
curriculum_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
experience_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
social_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  curriculum_experience_update_dto: OpenapiClient::CurriculumExperienceUpdateDto.new # CurriculumExperienceUpdateDto | 
}

begin
  # Update a curriculum experience
  result = api_instance.update_curriculum_experience_async(curriculum_id, experience_id, social_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->update_curriculum_experience_async: #{e}"
end
```

#### Using the update_curriculum_experience_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)

```ruby
begin
  # Update a curriculum experience
  data, status_code, headers = api_instance.update_curriculum_experience_async_with_http_info(curriculum_id, experience_id, social_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurriculumExperiencesApi->update_curriculum_experience_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curriculum_id** | **String** |  |  |
| **experience_id** | **String** |  |  |
| **social_profile_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **curriculum_experience_update_dto** | [**CurriculumExperienceUpdateDto**](CurriculumExperienceUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

