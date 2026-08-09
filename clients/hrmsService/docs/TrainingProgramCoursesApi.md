# OpenapiClient::TrainingProgramCoursesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_training_program_course_async**](TrainingProgramCoursesApi.md#create_training_program_course_async) | **POST** /api/v2/HrmsService/TrainingProgramCourses | Create a training program course |
| [**delete_training_program_course_async**](TrainingProgramCoursesApi.md#delete_training_program_course_async) | **DELETE** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Delete a training program course |
| [**get_training_program_course_by_id_async**](TrainingProgramCoursesApi.md#get_training_program_course_by_id_async) | **GET** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Get training program course by ID |
| [**get_training_program_courses_async**](TrainingProgramCoursesApi.md#get_training_program_courses_async) | **GET** /api/v2/HrmsService/TrainingProgramCourses | Get training program courses |
| [**get_training_program_courses_count_async**](TrainingProgramCoursesApi.md#get_training_program_courses_count_async) | **GET** /api/v2/HrmsService/TrainingProgramCourses/Count | Count training program courses |
| [**patch_training_program_course_async**](TrainingProgramCoursesApi.md#patch_training_program_course_async) | **PATCH** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Patch a training program course |
| [**update_training_program_course_async**](TrainingProgramCoursesApi.md#update_training_program_course_async) | **PUT** /api/v2/HrmsService/TrainingProgramCourses/{courseId} | Update a training program course |


## create_training_program_course_async

> <EmptyEnvelope> create_training_program_course_async(tenant_id, opts)

Create a training program course

Creates a new training program course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_course_create_dto: OpenapiClient::TrainingProgramCourseCreateDto.new({training_program_id: 'training_program_id_example', course_id: 'course_id_example'}) # TrainingProgramCourseCreateDto | 
}

begin
  # Create a training program course
  result = api_instance.create_training_program_course_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->create_training_program_course_async: #{e}"
end
```

#### Using the create_training_program_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_training_program_course_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a training program course
  data, status_code, headers = api_instance.create_training_program_course_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->create_training_program_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_course_create_dto** | [**TrainingProgramCourseCreateDto**](TrainingProgramCourseCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_training_program_course_async

> <EmptyEnvelope> delete_training_program_course_async(tenant_id, course_id, opts)

Delete a training program course

Deletes a training program course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a training program course
  result = api_instance.delete_training_program_course_async(tenant_id, course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->delete_training_program_course_async: #{e}"
end
```

#### Using the delete_training_program_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_training_program_course_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Delete a training program course
  data, status_code, headers = api_instance.delete_training_program_course_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->delete_training_program_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_program_course_by_id_async

> <TrainingProgramCourseDtoEnvelope> get_training_program_course_by_id_async(tenant_id, course_id, opts)

Get training program course by ID

Retrieves a specific training program course by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get training program course by ID
  result = api_instance.get_training_program_course_by_id_async(tenant_id, course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->get_training_program_course_by_id_async: #{e}"
end
```

#### Using the get_training_program_course_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrainingProgramCourseDtoEnvelope>, Integer, Hash)> get_training_program_course_by_id_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Get training program course by ID
  data, status_code, headers = api_instance.get_training_program_course_by_id_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrainingProgramCourseDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->get_training_program_course_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrainingProgramCourseDtoEnvelope**](TrainingProgramCourseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_training_program_courses_async

> <TrainingProgramCourseDtoListEnvelope> get_training_program_courses_async(tenant_id, opts)

Get training program courses

Retrieves training program courses for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_course_dto_collection_query_parameters: OpenapiClient::TrainingProgramCourseDtoCollectionQueryParameters.new # TrainingProgramCourseDtoCollectionQueryParameters | 
}

begin
  # Get training program courses
  result = api_instance.get_training_program_courses_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->get_training_program_courses_async: #{e}"
end
```

#### Using the get_training_program_courses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrainingProgramCourseDtoListEnvelope>, Integer, Hash)> get_training_program_courses_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get training program courses
  data, status_code, headers = api_instance.get_training_program_courses_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrainingProgramCourseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->get_training_program_courses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_course_dto_collection_query_parameters** | [**TrainingProgramCourseDtoCollectionQueryParameters**](TrainingProgramCourseDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**TrainingProgramCourseDtoListEnvelope**](TrainingProgramCourseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_training_program_courses_count_async

> <Int32Envelope> get_training_program_courses_count_async(tenant_id, opts)

Count training program courses

Counts training program courses for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_course_dto_collection_query_parameters: OpenapiClient::TrainingProgramCourseDtoCollectionQueryParameters.new # TrainingProgramCourseDtoCollectionQueryParameters | 
}

begin
  # Count training program courses
  result = api_instance.get_training_program_courses_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->get_training_program_courses_count_async: #{e}"
end
```

#### Using the get_training_program_courses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_training_program_courses_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count training program courses
  data, status_code, headers = api_instance.get_training_program_courses_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->get_training_program_courses_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_course_dto_collection_query_parameters** | [**TrainingProgramCourseDtoCollectionQueryParameters**](TrainingProgramCourseDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_training_program_course_async

> <EmptyEnvelope> patch_training_program_course_async(tenant_id, course_id, opts)

Patch a training program course

Partially updates an existing training program course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a training program course
  result = api_instance.patch_training_program_course_async(tenant_id, course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->patch_training_program_course_async: #{e}"
end
```

#### Using the patch_training_program_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_training_program_course_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Patch a training program course
  data, status_code, headers = api_instance.patch_training_program_course_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->patch_training_program_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
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


## update_training_program_course_async

> <EmptyEnvelope> update_training_program_course_async(tenant_id, course_id, opts)

Update a training program course

Updates an existing training program course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrainingProgramCoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  training_program_course_update_dto: OpenapiClient::TrainingProgramCourseUpdateDto.new # TrainingProgramCourseUpdateDto | 
}

begin
  # Update a training program course
  result = api_instance.update_training_program_course_async(tenant_id, course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->update_training_program_course_async: #{e}"
end
```

#### Using the update_training_program_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_training_program_course_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Update a training program course
  data, status_code, headers = api_instance.update_training_program_course_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrainingProgramCoursesApi->update_training_program_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **training_program_course_update_dto** | [**TrainingProgramCourseUpdateDto**](TrainingProgramCourseUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

