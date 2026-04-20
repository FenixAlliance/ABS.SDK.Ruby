# OpenapiClient::CourseHandoutsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_handout_async**](CourseHandoutsApi.md#create_course_handout_async) | **POST** /api/v2/LearningService/CourseHandouts | Create a course handout |
| [**delete_course_handout_async**](CourseHandoutsApi.md#delete_course_handout_async) | **DELETE** /api/v2/LearningService/CourseHandouts/{handoutId} | Delete a course handout |
| [**get_course_handout_by_id_async**](CourseHandoutsApi.md#get_course_handout_by_id_async) | **GET** /api/v2/LearningService/CourseHandouts/{handoutId} | Get course handout by ID |
| [**get_course_handouts_async**](CourseHandoutsApi.md#get_course_handouts_async) | **GET** /api/v2/LearningService/CourseHandouts | Get all course handouts |
| [**get_course_handouts_count_async**](CourseHandoutsApi.md#get_course_handouts_count_async) | **GET** /api/v2/LearningService/CourseHandouts/Count | Get course handouts count |
| [**update_course_handout_async**](CourseHandoutsApi.md#update_course_handout_async) | **PUT** /api/v2/LearningService/CourseHandouts/{handoutId} | Update a course handout |


## create_course_handout_async

> <CourseHandoutDto> create_course_handout_async(tenant_id, opts)

Create a course handout

Creates a new course handout for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseHandoutsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_handout_create_dto: OpenapiClient::CourseHandoutCreateDto.new({name: 'name_example', course_id: 'course_id_example'}) # CourseHandoutCreateDto | 
}

begin
  # Create a course handout
  result = api_instance.create_course_handout_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->create_course_handout_async: #{e}"
end
```

#### Using the create_course_handout_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseHandoutDto>, Integer, Hash)> create_course_handout_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course handout
  data, status_code, headers = api_instance.create_course_handout_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseHandoutDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->create_course_handout_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_handout_create_dto** | [**CourseHandoutCreateDto**](CourseHandoutCreateDto.md) |  | [optional] |

### Return type

[**CourseHandoutDto**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_handout_async

> delete_course_handout_async(tenant_id, handout_id, opts)

Delete a course handout

Deletes a course handout by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseHandoutsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
handout_id = 'handout_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course handout
  api_instance.delete_course_handout_async(tenant_id, handout_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->delete_course_handout_async: #{e}"
end
```

#### Using the delete_course_handout_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_handout_async_with_http_info(tenant_id, handout_id, opts)

```ruby
begin
  # Delete a course handout
  data, status_code, headers = api_instance.delete_course_handout_async_with_http_info(tenant_id, handout_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->delete_course_handout_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **handout_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_handout_by_id_async

> <CourseHandoutDto> get_course_handout_by_id_async(handout_id, opts)

Get course handout by ID

Retrieves a specific course handout by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseHandoutsApi.new
handout_id = 'handout_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course handout by ID
  result = api_instance.get_course_handout_by_id_async(handout_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->get_course_handout_by_id_async: #{e}"
end
```

#### Using the get_course_handout_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseHandoutDto>, Integer, Hash)> get_course_handout_by_id_async_with_http_info(handout_id, opts)

```ruby
begin
  # Get course handout by ID
  data, status_code, headers = api_instance.get_course_handout_by_id_async_with_http_info(handout_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseHandoutDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->get_course_handout_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **handout_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseHandoutDto**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_handouts_async

> <Array<CourseHandoutDto>> get_course_handouts_async(tenant_id, opts)

Get all course handouts

Retrieves all course handouts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseHandoutsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course handouts
  result = api_instance.get_course_handouts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->get_course_handouts_async: #{e}"
end
```

#### Using the get_course_handouts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseHandoutDto>>, Integer, Hash)> get_course_handouts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course handouts
  data, status_code, headers = api_instance.get_course_handouts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseHandoutDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->get_course_handouts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseHandoutDto&gt;**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_handouts_count_async

> Integer get_course_handouts_count_async(tenant_id, opts)

Get course handouts count

Returns the count of course handouts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseHandoutsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course handouts count
  result = api_instance.get_course_handouts_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->get_course_handouts_count_async: #{e}"
end
```

#### Using the get_course_handouts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_handouts_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course handouts count
  data, status_code, headers = api_instance.get_course_handouts_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->get_course_handouts_count_async_with_http_info: #{e}"
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


## update_course_handout_async

> <CourseHandoutDto> update_course_handout_async(tenant_id, handout_id, opts)

Update a course handout

Updates an existing course handout.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseHandoutsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
handout_id = 'handout_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_handout_update_dto: OpenapiClient::CourseHandoutUpdateDto.new # CourseHandoutUpdateDto | 
}

begin
  # Update a course handout
  result = api_instance.update_course_handout_async(tenant_id, handout_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->update_course_handout_async: #{e}"
end
```

#### Using the update_course_handout_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseHandoutDto>, Integer, Hash)> update_course_handout_async_with_http_info(tenant_id, handout_id, opts)

```ruby
begin
  # Update a course handout
  data, status_code, headers = api_instance.update_course_handout_async_with_http_info(tenant_id, handout_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseHandoutDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseHandoutsApi->update_course_handout_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **handout_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_handout_update_dto** | [**CourseHandoutUpdateDto**](CourseHandoutUpdateDto.md) |  | [optional] |

### Return type

[**CourseHandoutDto**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

