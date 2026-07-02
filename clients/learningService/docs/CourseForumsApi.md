# OpenapiClient::CourseForumsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_forum_async**](CourseForumsApi.md#create_course_forum_async) | **POST** /api/v2/LearningService/CourseForums | Create a course forum |
| [**delete_course_forum_async**](CourseForumsApi.md#delete_course_forum_async) | **DELETE** /api/v2/LearningService/CourseForums/{forumId} | Delete a course forum |
| [**get_course_forum_by_id_async**](CourseForumsApi.md#get_course_forum_by_id_async) | **GET** /api/v2/LearningService/CourseForums/{forumId} | Get course forum by ID |
| [**get_course_forums_async**](CourseForumsApi.md#get_course_forums_async) | **GET** /api/v2/LearningService/CourseForums | Get all course forums |
| [**get_course_forums_count_async**](CourseForumsApi.md#get_course_forums_count_async) | **GET** /api/v2/LearningService/CourseForums/Count | Get course forums count |
| [**patch_course_forum_async**](CourseForumsApi.md#patch_course_forum_async) | **PATCH** /api/v2/LearningService/CourseForums/{forumId} | Patch a course forum |
| [**update_course_forum_async**](CourseForumsApi.md#update_course_forum_async) | **PUT** /api/v2/LearningService/CourseForums/{forumId} | Update a course forum |


## create_course_forum_async

> <CourseForumDto> create_course_forum_async(tenant_id, opts)

Create a course forum

Creates a new course forum for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_forum_create_dto: OpenapiClient::CourseForumCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CourseForumCreateDto | 
}

begin
  # Create a course forum
  result = api_instance.create_course_forum_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->create_course_forum_async: #{e}"
end
```

#### Using the create_course_forum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseForumDto>, Integer, Hash)> create_course_forum_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course forum
  data, status_code, headers = api_instance.create_course_forum_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseForumDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->create_course_forum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_forum_create_dto** | [**CourseForumCreateDto**](CourseForumCreateDto.md) |  | [optional] |

### Return type

[**CourseForumDto**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_forum_async

> delete_course_forum_async(tenant_id, forum_id, opts)

Delete a course forum

Deletes a course forum by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
forum_id = 'forum_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course forum
  api_instance.delete_course_forum_async(tenant_id, forum_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->delete_course_forum_async: #{e}"
end
```

#### Using the delete_course_forum_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_forum_async_with_http_info(tenant_id, forum_id, opts)

```ruby
begin
  # Delete a course forum
  data, status_code, headers = api_instance.delete_course_forum_async_with_http_info(tenant_id, forum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->delete_course_forum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **forum_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_forum_by_id_async

> <CourseForumDto> get_course_forum_by_id_async(forum_id, opts)

Get course forum by ID

Retrieves a specific course forum by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
forum_id = 'forum_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course forum by ID
  result = api_instance.get_course_forum_by_id_async(forum_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->get_course_forum_by_id_async: #{e}"
end
```

#### Using the get_course_forum_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseForumDto>, Integer, Hash)> get_course_forum_by_id_async_with_http_info(forum_id, opts)

```ruby
begin
  # Get course forum by ID
  data, status_code, headers = api_instance.get_course_forum_by_id_async_with_http_info(forum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseForumDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->get_course_forum_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **forum_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseForumDto**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_forums_async

> <Array<CourseForumDto>> get_course_forums_async(tenant_id, opts)

Get all course forums

Retrieves all course forums for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course forums
  result = api_instance.get_course_forums_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->get_course_forums_async: #{e}"
end
```

#### Using the get_course_forums_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseForumDto>>, Integer, Hash)> get_course_forums_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course forums
  data, status_code, headers = api_instance.get_course_forums_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseForumDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->get_course_forums_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseForumDto&gt;**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_forums_count_async

> Integer get_course_forums_count_async(tenant_id, opts)

Get course forums count

Returns the count of course forums for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course forums count
  result = api_instance.get_course_forums_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->get_course_forums_count_async: #{e}"
end
```

#### Using the get_course_forums_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_forums_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course forums count
  data, status_code, headers = api_instance.get_course_forums_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->get_course_forums_count_async_with_http_info: #{e}"
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


## patch_course_forum_async

> patch_course_forum_async(tenant_id, forum_id, opts)

Patch a course forum

Partially updates an existing course forum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
forum_id = 'forum_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course forum
  api_instance.patch_course_forum_async(tenant_id, forum_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->patch_course_forum_async: #{e}"
end
```

#### Using the patch_course_forum_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_course_forum_async_with_http_info(tenant_id, forum_id, opts)

```ruby
begin
  # Patch a course forum
  data, status_code, headers = api_instance.patch_course_forum_async_with_http_info(tenant_id, forum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->patch_course_forum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **forum_id** | **String** |  |  |
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


## update_course_forum_async

> <CourseForumDto> update_course_forum_async(tenant_id, forum_id, opts)

Update a course forum

Updates an existing course forum.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseForumsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
forum_id = 'forum_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_forum_update_dto: OpenapiClient::CourseForumUpdateDto.new # CourseForumUpdateDto | 
}

begin
  # Update a course forum
  result = api_instance.update_course_forum_async(tenant_id, forum_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->update_course_forum_async: #{e}"
end
```

#### Using the update_course_forum_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseForumDto>, Integer, Hash)> update_course_forum_async_with_http_info(tenant_id, forum_id, opts)

```ruby
begin
  # Update a course forum
  data, status_code, headers = api_instance.update_course_forum_async_with_http_info(tenant_id, forum_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseForumDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseForumsApi->update_course_forum_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **forum_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_forum_update_dto** | [**CourseForumUpdateDto**](CourseForumUpdateDto.md) |  | [optional] |

### Return type

[**CourseForumDto**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

