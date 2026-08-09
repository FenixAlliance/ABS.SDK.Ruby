# OpenapiClient::CourseAssignmentTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_assignment_type_async**](CourseAssignmentTypesApi.md#create_course_assignment_type_async) | **POST** /api/v2/LearningService/CourseAssignmentTypes | Create a course assignment type |
| [**delete_course_assignment_type_async**](CourseAssignmentTypesApi.md#delete_course_assignment_type_async) | **DELETE** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Delete a course assignment type |
| [**get_course_assignment_type_by_id_async**](CourseAssignmentTypesApi.md#get_course_assignment_type_by_id_async) | **GET** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Get course assignment type by ID |
| [**get_course_assignment_types_async**](CourseAssignmentTypesApi.md#get_course_assignment_types_async) | **GET** /api/v2/LearningService/CourseAssignmentTypes | Get all course assignment types |
| [**get_course_assignment_types_count_async**](CourseAssignmentTypesApi.md#get_course_assignment_types_count_async) | **GET** /api/v2/LearningService/CourseAssignmentTypes/Count | Get course assignment types count |
| [**patch_course_assignment_type_async**](CourseAssignmentTypesApi.md#patch_course_assignment_type_async) | **PATCH** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Patch a course assignment type |
| [**update_course_assignment_type_async**](CourseAssignmentTypesApi.md#update_course_assignment_type_async) | **PUT** /api/v2/LearningService/CourseAssignmentTypes/{assignmentTypeId} | Update a course assignment type |


## create_course_assignment_type_async

> create_course_assignment_type_async(tenant_id, opts)

Create a course assignment type

Creates a new course assignment type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_assignment_type_create_dto: OpenapiClient::CourseAssignmentTypeCreateDto.new({name: 'name_example', course_id: 'course_id_example'}) # CourseAssignmentTypeCreateDto | 
}

begin
  # Create a course assignment type
  api_instance.create_course_assignment_type_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->create_course_assignment_type_async: #{e}"
end
```

#### Using the create_course_assignment_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_assignment_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course assignment type
  data, status_code, headers = api_instance.create_course_assignment_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->create_course_assignment_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_assignment_type_create_dto** | [**CourseAssignmentTypeCreateDto**](CourseAssignmentTypeCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_assignment_type_async

> delete_course_assignment_type_async(tenant_id, assignment_type_id, opts)

Delete a course assignment type

Deletes a course assignment type by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
assignment_type_id = 'assignment_type_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course assignment type
  api_instance.delete_course_assignment_type_async(tenant_id, assignment_type_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->delete_course_assignment_type_async: #{e}"
end
```

#### Using the delete_course_assignment_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_assignment_type_async_with_http_info(tenant_id, assignment_type_id, opts)

```ruby
begin
  # Delete a course assignment type
  data, status_code, headers = api_instance.delete_course_assignment_type_async_with_http_info(tenant_id, assignment_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->delete_course_assignment_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **assignment_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignment_type_by_id_async

> <CourseAssignmentTypeDto> get_course_assignment_type_by_id_async(assignment_type_id, opts)

Get course assignment type by ID

Retrieves a specific course assignment type by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
assignment_type_id = 'assignment_type_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course assignment type by ID
  result = api_instance.get_course_assignment_type_by_id_async(assignment_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->get_course_assignment_type_by_id_async: #{e}"
end
```

#### Using the get_course_assignment_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseAssignmentTypeDto>, Integer, Hash)> get_course_assignment_type_by_id_async_with_http_info(assignment_type_id, opts)

```ruby
begin
  # Get course assignment type by ID
  data, status_code, headers = api_instance.get_course_assignment_type_by_id_async_with_http_info(assignment_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseAssignmentTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->get_course_assignment_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **assignment_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseAssignmentTypeDto**](CourseAssignmentTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignment_types_async

> <Array<CourseAssignmentTypeDto>> get_course_assignment_types_async(tenant_id, opts)

Get all course assignment types

Retrieves all course assignment types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_assignment_type_dto_collection_query_parameters: OpenapiClient::CourseAssignmentTypeDtoCollectionQueryParameters.new # CourseAssignmentTypeDtoCollectionQueryParameters | 
}

begin
  # Get all course assignment types
  result = api_instance.get_course_assignment_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->get_course_assignment_types_async: #{e}"
end
```

#### Using the get_course_assignment_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseAssignmentTypeDto>>, Integer, Hash)> get_course_assignment_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course assignment types
  data, status_code, headers = api_instance.get_course_assignment_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseAssignmentTypeDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->get_course_assignment_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_assignment_type_dto_collection_query_parameters** | [**CourseAssignmentTypeDtoCollectionQueryParameters**](CourseAssignmentTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Array&lt;CourseAssignmentTypeDto&gt;**](CourseAssignmentTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_course_assignment_types_count_async

> Integer get_course_assignment_types_count_async(tenant_id, opts)

Get course assignment types count

Returns the count of course assignment types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_assignment_type_dto_collection_query_parameters: OpenapiClient::CourseAssignmentTypeDtoCollectionQueryParameters.new # CourseAssignmentTypeDtoCollectionQueryParameters | 
}

begin
  # Get course assignment types count
  result = api_instance.get_course_assignment_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->get_course_assignment_types_count_async: #{e}"
end
```

#### Using the get_course_assignment_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_assignment_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course assignment types count
  data, status_code, headers = api_instance.get_course_assignment_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->get_course_assignment_types_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_assignment_type_dto_collection_query_parameters** | [**CourseAssignmentTypeDtoCollectionQueryParameters**](CourseAssignmentTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_course_assignment_type_async

> <EmptyEnvelope> patch_course_assignment_type_async(tenant_id, assignment_type_id, opts)

Patch a course assignment type

Partially updates a course assignment type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
assignment_type_id = 'assignment_type_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a course assignment type
  result = api_instance.patch_course_assignment_type_async(tenant_id, assignment_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->patch_course_assignment_type_async: #{e}"
end
```

#### Using the patch_course_assignment_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_assignment_type_async_with_http_info(tenant_id, assignment_type_id, opts)

```ruby
begin
  # Patch a course assignment type
  data, status_code, headers = api_instance.patch_course_assignment_type_async_with_http_info(tenant_id, assignment_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->patch_course_assignment_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **assignment_type_id** | **String** |  |  |
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


## update_course_assignment_type_async

> update_course_assignment_type_async(tenant_id, assignment_type_id, opts)

Update a course assignment type

Updates an existing course assignment type.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
assignment_type_id = 'assignment_type_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_assignment_type_update_dto: OpenapiClient::CourseAssignmentTypeUpdateDto.new # CourseAssignmentTypeUpdateDto | 
}

begin
  # Update a course assignment type
  api_instance.update_course_assignment_type_async(tenant_id, assignment_type_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->update_course_assignment_type_async: #{e}"
end
```

#### Using the update_course_assignment_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_assignment_type_async_with_http_info(tenant_id, assignment_type_id, opts)

```ruby
begin
  # Update a course assignment type
  data, status_code, headers = api_instance.update_course_assignment_type_async_with_http_info(tenant_id, assignment_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentTypesApi->update_course_assignment_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **assignment_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_assignment_type_update_dto** | [**CourseAssignmentTypeUpdateDto**](CourseAssignmentTypeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

