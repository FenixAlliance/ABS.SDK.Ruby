# OpenapiClient::InstructorProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**api_v2_learning_service_instructor_profiles_count_get**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_count_get) | **GET** /api/v2/LearningService/InstructorProfiles/Count |  |
| [**api_v2_learning_service_instructor_profiles_get**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_get) | **GET** /api/v2/LearningService/InstructorProfiles |  |
| [**api_v2_learning_service_instructor_profiles_instructor_profile_id_delete**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_instructor_profile_id_delete) | **DELETE** /api/v2/LearningService/InstructorProfiles/{instructorProfileId} |  |
| [**api_v2_learning_service_instructor_profiles_instructor_profile_id_get**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_instructor_profile_id_get) | **GET** /api/v2/LearningService/InstructorProfiles/{instructorProfileId} |  |
| [**api_v2_learning_service_instructor_profiles_instructor_profile_id_put**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_instructor_profile_id_put) | **PUT** /api/v2/LearningService/InstructorProfiles/{instructorProfileId} |  |
| [**api_v2_learning_service_instructor_profiles_post**](InstructorProfilesApi.md#api_v2_learning_service_instructor_profiles_post) | **POST** /api/v2/LearningService/InstructorProfiles |  |


## api_v2_learning_service_instructor_profiles_count_get

> Integer api_v2_learning_service_instructor_profiles_count_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InstructorProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_instructor_profiles_count_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_count_get: #{e}"
end
```

#### Using the api_v2_learning_service_instructor_profiles_count_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> api_v2_learning_service_instructor_profiles_count_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_instructor_profiles_count_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_count_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_instructor_profiles_get

> <Array<InstructorProfileDto>> api_v2_learning_service_instructor_profiles_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InstructorProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_instructor_profiles_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_get: #{e}"
end
```

#### Using the api_v2_learning_service_instructor_profiles_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<InstructorProfileDto>>, Integer, Hash)> api_v2_learning_service_instructor_profiles_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_instructor_profiles_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<InstructorProfileDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;InstructorProfileDto&gt;**](InstructorProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_instructor_profiles_instructor_profile_id_delete

> api_v2_learning_service_instructor_profiles_instructor_profile_id_delete(tenant_id, instructor_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InstructorProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
instructor_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  api_instance.api_v2_learning_service_instructor_profiles_instructor_profile_id_delete(tenant_id, instructor_profile_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_instructor_profile_id_delete: #{e}"
end
```

#### Using the api_v2_learning_service_instructor_profiles_instructor_profile_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_learning_service_instructor_profiles_instructor_profile_id_delete_with_http_info(tenant_id, instructor_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_instructor_profiles_instructor_profile_id_delete_with_http_info(tenant_id, instructor_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_instructor_profile_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **instructor_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_instructor_profiles_instructor_profile_id_get

> <InstructorProfileDto> api_v2_learning_service_instructor_profiles_instructor_profile_id_get(tenant_id, instructor_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InstructorProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
instructor_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_instructor_profiles_instructor_profile_id_get(tenant_id, instructor_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_instructor_profile_id_get: #{e}"
end
```

#### Using the api_v2_learning_service_instructor_profiles_instructor_profile_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InstructorProfileDto>, Integer, Hash)> api_v2_learning_service_instructor_profiles_instructor_profile_id_get_with_http_info(tenant_id, instructor_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_instructor_profiles_instructor_profile_id_get_with_http_info(tenant_id, instructor_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InstructorProfileDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_instructor_profile_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **instructor_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InstructorProfileDto**](InstructorProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_instructor_profiles_instructor_profile_id_put

> api_v2_learning_service_instructor_profiles_instructor_profile_id_put(tenant_id, instructor_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InstructorProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
instructor_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  instructor_profile_update_dto: OpenapiClient::InstructorProfileUpdateDto.new # InstructorProfileUpdateDto | 
}

begin
  
  api_instance.api_v2_learning_service_instructor_profiles_instructor_profile_id_put(tenant_id, instructor_profile_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_instructor_profile_id_put: #{e}"
end
```

#### Using the api_v2_learning_service_instructor_profiles_instructor_profile_id_put_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_learning_service_instructor_profiles_instructor_profile_id_put_with_http_info(tenant_id, instructor_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_instructor_profiles_instructor_profile_id_put_with_http_info(tenant_id, instructor_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_instructor_profile_id_put_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **instructor_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **instructor_profile_update_dto** | [**InstructorProfileUpdateDto**](InstructorProfileUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## api_v2_learning_service_instructor_profiles_post

> api_v2_learning_service_instructor_profiles_post(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::InstructorProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  instructor_profile_create_dto: OpenapiClient::InstructorProfileCreateDto.new # InstructorProfileCreateDto | 
}

begin
  
  api_instance.api_v2_learning_service_instructor_profiles_post(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_post: #{e}"
end
```

#### Using the api_v2_learning_service_instructor_profiles_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_learning_service_instructor_profiles_post_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_instructor_profiles_post_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling InstructorProfilesApi->api_v2_learning_service_instructor_profiles_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **instructor_profile_create_dto** | [**InstructorProfileCreateDto**](InstructorProfileCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

