# OpenapiClient::CourseLibrariesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_library_async**](CourseLibrariesApi.md#create_course_library_async) | **POST** /api/v2/LearningService/CourseLibraries | Create a course library |
| [**delete_course_library_async**](CourseLibrariesApi.md#delete_course_library_async) | **DELETE** /api/v2/LearningService/CourseLibraries/{libraryId} | Delete a course library |
| [**get_course_libraries_async**](CourseLibrariesApi.md#get_course_libraries_async) | **GET** /api/v2/LearningService/CourseLibraries | Get all course libraries |
| [**get_course_libraries_count_async**](CourseLibrariesApi.md#get_course_libraries_count_async) | **GET** /api/v2/LearningService/CourseLibraries/Count | Get course libraries count |
| [**get_course_library_by_id_async**](CourseLibrariesApi.md#get_course_library_by_id_async) | **GET** /api/v2/LearningService/CourseLibraries/{libraryId} | Get course library by ID |
| [**update_course_library_async**](CourseLibrariesApi.md#update_course_library_async) | **PUT** /api/v2/LearningService/CourseLibraries/{libraryId} | Update a course library |


## create_course_library_async

> <CourseLibraryDto> create_course_library_async(tenant_id, opts)

Create a course library

Creates a new course library for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseLibrariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_library_create_dto: OpenapiClient::CourseLibraryCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CourseLibraryCreateDto | 
}

begin
  # Create a course library
  result = api_instance.create_course_library_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->create_course_library_async: #{e}"
end
```

#### Using the create_course_library_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseLibraryDto>, Integer, Hash)> create_course_library_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course library
  data, status_code, headers = api_instance.create_course_library_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseLibraryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->create_course_library_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_library_create_dto** | [**CourseLibraryCreateDto**](CourseLibraryCreateDto.md) |  | [optional] |

### Return type

[**CourseLibraryDto**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_library_async

> delete_course_library_async(tenant_id, library_id, opts)

Delete a course library

Deletes a course library by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseLibrariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
library_id = 'library_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course library
  api_instance.delete_course_library_async(tenant_id, library_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->delete_course_library_async: #{e}"
end
```

#### Using the delete_course_library_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_library_async_with_http_info(tenant_id, library_id, opts)

```ruby
begin
  # Delete a course library
  data, status_code, headers = api_instance.delete_course_library_async_with_http_info(tenant_id, library_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->delete_course_library_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **library_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_libraries_async

> <Array<CourseLibraryDto>> get_course_libraries_async(tenant_id, opts)

Get all course libraries

Retrieves all course libraries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseLibrariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course libraries
  result = api_instance.get_course_libraries_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->get_course_libraries_async: #{e}"
end
```

#### Using the get_course_libraries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseLibraryDto>>, Integer, Hash)> get_course_libraries_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course libraries
  data, status_code, headers = api_instance.get_course_libraries_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseLibraryDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->get_course_libraries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseLibraryDto&gt;**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_libraries_count_async

> Integer get_course_libraries_count_async(tenant_id, opts)

Get course libraries count

Returns the count of course libraries for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseLibrariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course libraries count
  result = api_instance.get_course_libraries_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->get_course_libraries_count_async: #{e}"
end
```

#### Using the get_course_libraries_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_libraries_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course libraries count
  data, status_code, headers = api_instance.get_course_libraries_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->get_course_libraries_count_async_with_http_info: #{e}"
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


## get_course_library_by_id_async

> <CourseLibraryDto> get_course_library_by_id_async(library_id, opts)

Get course library by ID

Retrieves a specific course library by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseLibrariesApi.new
library_id = 'library_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course library by ID
  result = api_instance.get_course_library_by_id_async(library_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->get_course_library_by_id_async: #{e}"
end
```

#### Using the get_course_library_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseLibraryDto>, Integer, Hash)> get_course_library_by_id_async_with_http_info(library_id, opts)

```ruby
begin
  # Get course library by ID
  data, status_code, headers = api_instance.get_course_library_by_id_async_with_http_info(library_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseLibraryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->get_course_library_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **library_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseLibraryDto**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_course_library_async

> <CourseLibraryDto> update_course_library_async(tenant_id, library_id, opts)

Update a course library

Updates an existing course library.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseLibrariesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
library_id = 'library_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_library_update_dto: OpenapiClient::CourseLibraryUpdateDto.new # CourseLibraryUpdateDto | 
}

begin
  # Update a course library
  result = api_instance.update_course_library_async(tenant_id, library_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->update_course_library_async: #{e}"
end
```

#### Using the update_course_library_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseLibraryDto>, Integer, Hash)> update_course_library_async_with_http_info(tenant_id, library_id, opts)

```ruby
begin
  # Update a course library
  data, status_code, headers = api_instance.update_course_library_async_with_http_info(tenant_id, library_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseLibraryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseLibrariesApi->update_course_library_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **library_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_library_update_dto** | [**CourseLibraryUpdateDto**](CourseLibraryUpdateDto.md) |  | [optional] |

### Return type

[**CourseLibraryDto**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

