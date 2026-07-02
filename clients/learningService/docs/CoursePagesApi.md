# OpenapiClient::CoursePagesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_page_async**](CoursePagesApi.md#create_course_page_async) | **POST** /api/v2/LearningService/CoursePages | Create a new course page |
| [**delete_course_page_async**](CoursePagesApi.md#delete_course_page_async) | **DELETE** /api/v2/LearningService/CoursePages/{pageId} | Delete a course page |
| [**get_course_page_by_id_async**](CoursePagesApi.md#get_course_page_by_id_async) | **GET** /api/v2/LearningService/CoursePages/{pageId} | Get course page by ID |
| [**get_course_pages_async**](CoursePagesApi.md#get_course_pages_async) | **GET** /api/v2/LearningService/CoursePages | Get all course pages |
| [**get_course_pages_count_async**](CoursePagesApi.md#get_course_pages_count_async) | **GET** /api/v2/LearningService/CoursePages/Count | Get course pages count |
| [**patch_course_page_async**](CoursePagesApi.md#patch_course_page_async) | **PATCH** /api/v2/LearningService/CoursePages/{pageId} | Patch a course page |
| [**update_course_page_async**](CoursePagesApi.md#update_course_page_async) | **PUT** /api/v2/LearningService/CoursePages/{pageId} | Update a course page |


## create_course_page_async

> create_course_page_async(tenant_id, opts)

Create a new course page

Creates a new course page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_page_create_dto: OpenapiClient::CoursePageCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CoursePageCreateDto | 
}

begin
  # Create a new course page
  api_instance.create_course_page_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->create_course_page_async: #{e}"
end
```

#### Using the create_course_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_page_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course page
  data, status_code, headers = api_instance.create_course_page_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->create_course_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_page_create_dto** | [**CoursePageCreateDto**](CoursePageCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_page_async

> delete_course_page_async(tenant_id, page_id, opts)

Delete a course page

Deletes a course page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
page_id = 'page_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course page
  api_instance.delete_course_page_async(tenant_id, page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->delete_course_page_async: #{e}"
end
```

#### Using the delete_course_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_page_async_with_http_info(tenant_id, page_id, opts)

```ruby
begin
  # Delete a course page
  data, status_code, headers = api_instance.delete_course_page_async_with_http_info(tenant_id, page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->delete_course_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_page_by_id_async

> <CoursePageDto> get_course_page_by_id_async(page_id, opts)

Get course page by ID

Retrieves a specific course page by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
page_id = 'page_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course page by ID
  result = api_instance.get_course_page_by_id_async(page_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->get_course_page_by_id_async: #{e}"
end
```

#### Using the get_course_page_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CoursePageDto>, Integer, Hash)> get_course_page_by_id_async_with_http_info(page_id, opts)

```ruby
begin
  # Get course page by ID
  data, status_code, headers = api_instance.get_course_page_by_id_async_with_http_info(page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CoursePageDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->get_course_page_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CoursePageDto**](CoursePageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_pages_async

> <Array<CoursePageDto>> get_course_pages_async(tenant_id, opts)

Get all course pages

Retrieves all course pages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course pages
  result = api_instance.get_course_pages_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->get_course_pages_async: #{e}"
end
```

#### Using the get_course_pages_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CoursePageDto>>, Integer, Hash)> get_course_pages_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course pages
  data, status_code, headers = api_instance.get_course_pages_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CoursePageDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->get_course_pages_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CoursePageDto&gt;**](CoursePageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_pages_count_async

> Integer get_course_pages_count_async(tenant_id, opts)

Get course pages count

Returns the count of course pages for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course pages count
  result = api_instance.get_course_pages_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->get_course_pages_count_async: #{e}"
end
```

#### Using the get_course_pages_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_pages_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course pages count
  data, status_code, headers = api_instance.get_course_pages_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->get_course_pages_count_async_with_http_info: #{e}"
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


## patch_course_page_async

> patch_course_page_async(tenant_id, page_id, opts)

Patch a course page

Partially updates an existing course page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
page_id = 'page_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course page
  api_instance.patch_course_page_async(tenant_id, page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->patch_course_page_async: #{e}"
end
```

#### Using the patch_course_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_course_page_async_with_http_info(tenant_id, page_id, opts)

```ruby
begin
  # Patch a course page
  data, status_code, headers = api_instance.patch_course_page_async_with_http_info(tenant_id, page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->patch_course_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_course_page_async

> update_course_page_async(tenant_id, page_id, opts)

Update a course page

Updates an existing course page for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursePagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
page_id = 'page_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_page_update_dto: OpenapiClient::CoursePageUpdateDto.new # CoursePageUpdateDto | 
}

begin
  # Update a course page
  api_instance.update_course_page_async(tenant_id, page_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->update_course_page_async: #{e}"
end
```

#### Using the update_course_page_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_page_async_with_http_info(tenant_id, page_id, opts)

```ruby
begin
  # Update a course page
  data, status_code, headers = api_instance.update_course_page_async_with_http_info(tenant_id, page_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursePagesApi->update_course_page_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **page_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_page_update_dto** | [**CoursePageUpdateDto**](CoursePageUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

