# OpenapiClient::CourseFilesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_file_async**](CourseFilesApi.md#create_course_file_async) | **POST** /api/v2/LearningService/CourseFiles | Create a new course file |
| [**delete_course_file_async**](CourseFilesApi.md#delete_course_file_async) | **DELETE** /api/v2/LearningService/CourseFiles/{fileId} | Delete a course file |
| [**get_course_file_by_id_async**](CourseFilesApi.md#get_course_file_by_id_async) | **GET** /api/v2/LearningService/CourseFiles/{fileId} | Get course file by ID |
| [**get_course_files_async**](CourseFilesApi.md#get_course_files_async) | **GET** /api/v2/LearningService/CourseFiles | Get all course files |
| [**get_course_files_count_async**](CourseFilesApi.md#get_course_files_count_async) | **GET** /api/v2/LearningService/CourseFiles/Count | Get course files count |
| [**update_course_file_async**](CourseFilesApi.md#update_course_file_async) | **PUT** /api/v2/LearningService/CourseFiles/{fileId} | Update a course file |


## create_course_file_async

> create_course_file_async(tenant_id, opts)

Create a new course file

Creates a new course file for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseFilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_file_create_dto: OpenapiClient::CourseFileCreateDto.new({title: 'title_example', file_name: 'file_name_example', file_upload_url: 'file_upload_url_example', course_id: 'course_id_example'}) # CourseFileCreateDto | 
}

begin
  # Create a new course file
  api_instance.create_course_file_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->create_course_file_async: #{e}"
end
```

#### Using the create_course_file_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_file_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course file
  data, status_code, headers = api_instance.create_course_file_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->create_course_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_file_create_dto** | [**CourseFileCreateDto**](CourseFileCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_file_async

> delete_course_file_async(tenant_id, file_id, opts)

Delete a course file

Deletes a course file for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseFilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
file_id = 'file_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course file
  api_instance.delete_course_file_async(tenant_id, file_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->delete_course_file_async: #{e}"
end
```

#### Using the delete_course_file_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_file_async_with_http_info(tenant_id, file_id, opts)

```ruby
begin
  # Delete a course file
  data, status_code, headers = api_instance.delete_course_file_async_with_http_info(tenant_id, file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->delete_course_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **file_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_file_by_id_async

> <CourseFileDto> get_course_file_by_id_async(file_id, opts)

Get course file by ID

Retrieves a specific course file by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseFilesApi.new
file_id = 'file_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course file by ID
  result = api_instance.get_course_file_by_id_async(file_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->get_course_file_by_id_async: #{e}"
end
```

#### Using the get_course_file_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseFileDto>, Integer, Hash)> get_course_file_by_id_async_with_http_info(file_id, opts)

```ruby
begin
  # Get course file by ID
  data, status_code, headers = api_instance.get_course_file_by_id_async_with_http_info(file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseFileDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->get_course_file_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseFileDto**](CourseFileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_files_async

> <Array<CourseFileDto>> get_course_files_async(tenant_id, opts)

Get all course files

Retrieves all course files for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseFilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course files
  result = api_instance.get_course_files_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->get_course_files_async: #{e}"
end
```

#### Using the get_course_files_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseFileDto>>, Integer, Hash)> get_course_files_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course files
  data, status_code, headers = api_instance.get_course_files_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseFileDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->get_course_files_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseFileDto&gt;**](CourseFileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_files_count_async

> Integer get_course_files_count_async(tenant_id, opts)

Get course files count

Returns the count of course files for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseFilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course files count
  result = api_instance.get_course_files_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->get_course_files_count_async: #{e}"
end
```

#### Using the get_course_files_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_files_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course files count
  data, status_code, headers = api_instance.get_course_files_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->get_course_files_count_async_with_http_info: #{e}"
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


## update_course_file_async

> update_course_file_async(tenant_id, file_id, opts)

Update a course file

Updates an existing course file for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseFilesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
file_id = 'file_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_file_update_dto: OpenapiClient::CourseFileUpdateDto.new # CourseFileUpdateDto | 
}

begin
  # Update a course file
  api_instance.update_course_file_async(tenant_id, file_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->update_course_file_async: #{e}"
end
```

#### Using the update_course_file_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_file_async_with_http_info(tenant_id, file_id, opts)

```ruby
begin
  # Update a course file
  data, status_code, headers = api_instance.update_course_file_async_with_http_info(tenant_id, file_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseFilesApi->update_course_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **file_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_file_update_dto** | [**CourseFileUpdateDto**](CourseFileUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

