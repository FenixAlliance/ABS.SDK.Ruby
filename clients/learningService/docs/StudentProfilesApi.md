# OpenapiClient::StudentProfilesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**api_v2_learning_service_student_profiles_count_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_count_get) | **GET** /api/v2/LearningService/StudentProfiles/Count |  |
| [**api_v2_learning_service_student_profiles_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_get) | **GET** /api/v2/LearningService/StudentProfiles |  |
| [**api_v2_learning_service_student_profiles_post**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_post) | **POST** /api/v2/LearningService/StudentProfiles |  |
| [**api_v2_learning_service_student_profiles_student_profile_id_average_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_average_get) | **GET** /api/v2/LearningService/StudentProfiles/{studentProfileId}/Average |  |
| [**api_v2_learning_service_student_profiles_student_profile_id_delete**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_delete) | **DELETE** /api/v2/LearningService/StudentProfiles/{studentProfileId} |  |
| [**api_v2_learning_service_student_profiles_student_profile_id_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_get) | **GET** /api/v2/LearningService/StudentProfiles/{studentProfileId} |  |
| [**api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get) | **GET** /api/v2/LearningService/StudentProfiles/{studentProfileId}/HoursCompleted |  |
| [**api_v2_learning_service_student_profiles_student_profile_id_patch**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_patch) | **PATCH** /api/v2/LearningService/StudentProfiles/{studentProfileId} |  |
| [**api_v2_learning_service_student_profiles_student_profile_id_put**](StudentProfilesApi.md#api_v2_learning_service_student_profiles_student_profile_id_put) | **PUT** /api/v2/LearningService/StudentProfiles/{studentProfileId} |  |


## api_v2_learning_service_student_profiles_count_get

> Integer api_v2_learning_service_student_profiles_count_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_student_profiles_count_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_count_get: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_count_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> api_v2_learning_service_student_profiles_count_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_count_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_count_get_with_http_info: #{e}"
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


## api_v2_learning_service_student_profiles_get

> <Array<StudentProfileDto>> api_v2_learning_service_student_profiles_get(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_student_profiles_get(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_get: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<StudentProfileDto>>, Integer, Hash)> api_v2_learning_service_student_profiles_get_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_get_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<StudentProfileDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;StudentProfileDto&gt;**](StudentProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_student_profiles_post

> api_v2_learning_service_student_profiles_post(tenant_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  student_profile_create_dto: OpenapiClient::StudentProfileCreateDto.new # StudentProfileCreateDto | 
}

begin
  
  api_instance.api_v2_learning_service_student_profiles_post(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_post: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_post_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_learning_service_student_profiles_post_with_http_info(tenant_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_post_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **student_profile_create_dto** | [**StudentProfileCreateDto**](StudentProfileCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## api_v2_learning_service_student_profiles_student_profile_id_average_get

> <AverageDto> api_v2_learning_service_student_profiles_student_profile_id_average_get(tenant_id, student_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_student_profiles_student_profile_id_average_get(tenant_id, student_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_average_get: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_student_profile_id_average_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AverageDto>, Integer, Hash)> api_v2_learning_service_student_profiles_student_profile_id_average_get_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_student_profile_id_average_get_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AverageDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_average_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AverageDto**](AverageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_student_profiles_student_profile_id_delete

> api_v2_learning_service_student_profiles_student_profile_id_delete(tenant_id, student_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  api_instance.api_v2_learning_service_student_profiles_student_profile_id_delete(tenant_id, student_profile_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_delete: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_student_profile_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_learning_service_student_profiles_student_profile_id_delete_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_student_profile_id_delete_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_student_profiles_student_profile_id_get

> <StudentProfileDto> api_v2_learning_service_student_profiles_student_profile_id_get(tenant_id, student_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_student_profiles_student_profile_id_get(tenant_id, student_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_get: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_student_profile_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StudentProfileDto>, Integer, Hash)> api_v2_learning_service_student_profiles_student_profile_id_get_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_student_profile_id_get_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StudentProfileDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**StudentProfileDto**](StudentProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get

> <CountDto> api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get(tenant_id, student_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  
  result = api_instance.api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get(tenant_id, student_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountDto>, Integer, Hash)> api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_hours_completed_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountDto**](CountDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## api_v2_learning_service_student_profiles_student_profile_id_patch

> <EmptyEnvelope> api_v2_learning_service_student_profiles_student_profile_id_patch(tenant_id, student_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  
  result = api_instance.api_v2_learning_service_student_profiles_student_profile_id_patch(tenant_id, student_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_patch: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_student_profile_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> api_v2_learning_service_student_profiles_student_profile_id_patch_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_student_profile_id_patch_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
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


## api_v2_learning_service_student_profiles_student_profile_id_put

> api_v2_learning_service_student_profiles_student_profile_id_put(tenant_id, student_profile_id, opts)



### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StudentProfilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  student_profile_update_dto: OpenapiClient::StudentProfileUpdateDto.new # StudentProfileUpdateDto | 
}

begin
  
  api_instance.api_v2_learning_service_student_profiles_student_profile_id_put(tenant_id, student_profile_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_put: #{e}"
end
```

#### Using the api_v2_learning_service_student_profiles_student_profile_id_put_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> api_v2_learning_service_student_profiles_student_profile_id_put_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.api_v2_learning_service_student_profiles_student_profile_id_put_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling StudentProfilesApi->api_v2_learning_service_student_profiles_student_profile_id_put_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **student_profile_update_dto** | [**StudentProfileUpdateDto**](StudentProfileUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

