# OpenapiClient::CourseAssignmentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_assignment_async**](CourseAssignmentsApi.md#create_course_assignment_async) | **POST** /api/v2/LearningService/CourseAssignments | Create a new course assignment |
| [**delete_course_assignment_async**](CourseAssignmentsApi.md#delete_course_assignment_async) | **DELETE** /api/v2/LearningService/CourseAssignments/{assignmentId} | Delete a course assignment |
| [**get_course_assignment_by_id_async**](CourseAssignmentsApi.md#get_course_assignment_by_id_async) | **GET** /api/v2/LearningService/CourseAssignments/{assignmentId} | Get course assignment by ID |
| [**get_course_assignments_async**](CourseAssignmentsApi.md#get_course_assignments_async) | **GET** /api/v2/LearningService/CourseAssignments | Get all course assignments |
| [**get_course_assignments_count_async**](CourseAssignmentsApi.md#get_course_assignments_count_async) | **GET** /api/v2/LearningService/CourseAssignments/Count | Get course assignments count |
| [**update_course_assignment_async**](CourseAssignmentsApi.md#update_course_assignment_async) | **PUT** /api/v2/LearningService/CourseAssignments/{assignmentId} | Update a course assignment |


## create_course_assignment_async

> create_course_assignment_async(tenant_id, opts)

Create a new course assignment

Creates a new course assignment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_assignment_create_dto: OpenapiClient::CourseAssignmentCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CourseAssignmentCreateDto | 
}

begin
  # Create a new course assignment
  api_instance.create_course_assignment_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->create_course_assignment_async: #{e}"
end
```

#### Using the create_course_assignment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_assignment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course assignment
  data, status_code, headers = api_instance.create_course_assignment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->create_course_assignment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_assignment_create_dto** | [**CourseAssignmentCreateDto**](CourseAssignmentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_assignment_async

> delete_course_assignment_async(tenant_id, assignment_id, opts)

Delete a course assignment

Deletes a course assignment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
assignment_id = 'assignment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course assignment
  api_instance.delete_course_assignment_async(tenant_id, assignment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->delete_course_assignment_async: #{e}"
end
```

#### Using the delete_course_assignment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_assignment_async_with_http_info(tenant_id, assignment_id, opts)

```ruby
begin
  # Delete a course assignment
  data, status_code, headers = api_instance.delete_course_assignment_async_with_http_info(tenant_id, assignment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->delete_course_assignment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **assignment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignment_by_id_async

> <CourseAssignmentDto> get_course_assignment_by_id_async(assignment_id, opts)

Get course assignment by ID

Retrieves a specific course assignment by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentsApi.new
assignment_id = 'assignment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course assignment by ID
  result = api_instance.get_course_assignment_by_id_async(assignment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->get_course_assignment_by_id_async: #{e}"
end
```

#### Using the get_course_assignment_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseAssignmentDto>, Integer, Hash)> get_course_assignment_by_id_async_with_http_info(assignment_id, opts)

```ruby
begin
  # Get course assignment by ID
  data, status_code, headers = api_instance.get_course_assignment_by_id_async_with_http_info(assignment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseAssignmentDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->get_course_assignment_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **assignment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseAssignmentDto**](CourseAssignmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignments_async

> <Array<CourseAssignmentDto>> get_course_assignments_async(tenant_id, opts)

Get all course assignments

Retrieves all course assignments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course assignments
  result = api_instance.get_course_assignments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->get_course_assignments_async: #{e}"
end
```

#### Using the get_course_assignments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseAssignmentDto>>, Integer, Hash)> get_course_assignments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course assignments
  data, status_code, headers = api_instance.get_course_assignments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseAssignmentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->get_course_assignments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseAssignmentDto&gt;**](CourseAssignmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignments_count_async

> Integer get_course_assignments_count_async(tenant_id, opts)

Get course assignments count

Returns the count of course assignments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course assignments count
  result = api_instance.get_course_assignments_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->get_course_assignments_count_async: #{e}"
end
```

#### Using the get_course_assignments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_assignments_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course assignments count
  data, status_code, headers = api_instance.get_course_assignments_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->get_course_assignments_count_async_with_http_info: #{e}"
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


## update_course_assignment_async

> update_course_assignment_async(tenant_id, assignment_id, opts)

Update a course assignment

Updates an existing course assignment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseAssignmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
assignment_id = 'assignment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_assignment_update_dto: OpenapiClient::CourseAssignmentUpdateDto.new # CourseAssignmentUpdateDto | 
}

begin
  # Update a course assignment
  api_instance.update_course_assignment_async(tenant_id, assignment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->update_course_assignment_async: #{e}"
end
```

#### Using the update_course_assignment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_assignment_async_with_http_info(tenant_id, assignment_id, opts)

```ruby
begin
  # Update a course assignment
  data, status_code, headers = api_instance.update_course_assignment_async_with_http_info(tenant_id, assignment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseAssignmentsApi->update_course_assignment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **assignment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_assignment_update_dto** | [**CourseAssignmentUpdateDto**](CourseAssignmentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

