# OpenapiClient::CourseUpdatesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_update_async**](CourseUpdatesApi.md#create_course_update_async) | **POST** /api/v2/LearningService/CourseUpdates | Create a new course update |
| [**delete_course_update_async**](CourseUpdatesApi.md#delete_course_update_async) | **DELETE** /api/v2/LearningService/CourseUpdates/{updateId} | Delete a course update |
| [**get_course_update_by_id_async**](CourseUpdatesApi.md#get_course_update_by_id_async) | **GET** /api/v2/LearningService/CourseUpdates/{updateId} | Get course update by ID |
| [**get_course_updates_async**](CourseUpdatesApi.md#get_course_updates_async) | **GET** /api/v2/LearningService/CourseUpdates | Get all course updates |
| [**get_course_updates_count_async**](CourseUpdatesApi.md#get_course_updates_count_async) | **GET** /api/v2/LearningService/CourseUpdates/Count | Get course updates count |
| [**update_course_update_async**](CourseUpdatesApi.md#update_course_update_async) | **PUT** /api/v2/LearningService/CourseUpdates/{updateId} | Update a course update |


## create_course_update_async

> create_course_update_async(tenant_id, opts)

Create a new course update

Creates a new course update for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUpdatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_news_create_dto: OpenapiClient::CourseNewsCreateDto.new({title: 'title_example', course_id: 'course_id_example', business_id: 'business_id_example'}) # CourseNewsCreateDto | 
}

begin
  # Create a new course update
  api_instance.create_course_update_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->create_course_update_async: #{e}"
end
```

#### Using the create_course_update_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_update_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course update
  data, status_code, headers = api_instance.create_course_update_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->create_course_update_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_news_create_dto** | [**CourseNewsCreateDto**](CourseNewsCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_update_async

> delete_course_update_async(tenant_id, update_id, opts)

Delete a course update

Deletes a course update for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUpdatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
update_id = 'update_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course update
  api_instance.delete_course_update_async(tenant_id, update_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->delete_course_update_async: #{e}"
end
```

#### Using the delete_course_update_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_update_async_with_http_info(tenant_id, update_id, opts)

```ruby
begin
  # Delete a course update
  data, status_code, headers = api_instance.delete_course_update_async_with_http_info(tenant_id, update_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->delete_course_update_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **update_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_update_by_id_async

> <CourseNewsDto> get_course_update_by_id_async(update_id, opts)

Get course update by ID

Retrieves a specific course update by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUpdatesApi.new
update_id = 'update_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course update by ID
  result = api_instance.get_course_update_by_id_async(update_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->get_course_update_by_id_async: #{e}"
end
```

#### Using the get_course_update_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseNewsDto>, Integer, Hash)> get_course_update_by_id_async_with_http_info(update_id, opts)

```ruby
begin
  # Get course update by ID
  data, status_code, headers = api_instance.get_course_update_by_id_async_with_http_info(update_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseNewsDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->get_course_update_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **update_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseNewsDto**](CourseNewsDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_updates_async

> <Array<CourseNewsDto>> get_course_updates_async(tenant_id, opts)

Get all course updates

Retrieves all course updates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUpdatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course updates
  result = api_instance.get_course_updates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->get_course_updates_async: #{e}"
end
```

#### Using the get_course_updates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseNewsDto>>, Integer, Hash)> get_course_updates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course updates
  data, status_code, headers = api_instance.get_course_updates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseNewsDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->get_course_updates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseNewsDto&gt;**](CourseNewsDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_updates_count_async

> Integer get_course_updates_count_async(tenant_id, opts)

Get course updates count

Returns the count of course updates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUpdatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course updates count
  result = api_instance.get_course_updates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->get_course_updates_count_async: #{e}"
end
```

#### Using the get_course_updates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_updates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course updates count
  data, status_code, headers = api_instance.get_course_updates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->get_course_updates_count_async_with_http_info: #{e}"
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


## update_course_update_async

> update_course_update_async(tenant_id, update_id, opts)

Update a course update

Updates an existing course update for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUpdatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
update_id = 'update_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_news_update_dto: OpenapiClient::CourseNewsUpdateDto.new # CourseNewsUpdateDto | 
}

begin
  # Update a course update
  api_instance.update_course_update_async(tenant_id, update_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->update_course_update_async: #{e}"
end
```

#### Using the update_course_update_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_update_async_with_http_info(tenant_id, update_id, opts)

```ruby
begin
  # Update a course update
  data, status_code, headers = api_instance.update_course_update_async_with_http_info(tenant_id, update_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUpdatesApi->update_course_update_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **update_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_news_update_dto** | [**CourseNewsUpdateDto**](CourseNewsUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

