# OpenapiClient::CourseContentGroupsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_content_group_async**](CourseContentGroupsApi.md#create_course_content_group_async) | **POST** /api/v2/LearningService/CourseContentGroups | Create a new course content group |
| [**delete_course_content_group_async**](CourseContentGroupsApi.md#delete_course_content_group_async) | **DELETE** /api/v2/LearningService/CourseContentGroups/{groupId} | Delete a course content group |
| [**get_course_content_group_by_id_async**](CourseContentGroupsApi.md#get_course_content_group_by_id_async) | **GET** /api/v2/LearningService/CourseContentGroups/{groupId} | Get course content group by ID |
| [**get_course_content_groups_async**](CourseContentGroupsApi.md#get_course_content_groups_async) | **GET** /api/v2/LearningService/CourseContentGroups | Get all course content groups |
| [**get_course_content_groups_by_course_async**](CourseContentGroupsApi.md#get_course_content_groups_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ContentGroups | Get course content groups by course |
| [**get_course_content_groups_by_course_count_async**](CourseContentGroupsApi.md#get_course_content_groups_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ContentGroups/Count | Get course content groups count by course |
| [**get_course_content_groups_count_async**](CourseContentGroupsApi.md#get_course_content_groups_count_async) | **GET** /api/v2/LearningService/CourseContentGroups/Count | Get course content groups count |
| [**update_course_content_group_async**](CourseContentGroupsApi.md#update_course_content_group_async) | **PUT** /api/v2/LearningService/CourseContentGroups/{groupId} | Update a course content group |


## create_course_content_group_async

> create_course_content_group_async(tenant_id, opts)

Create a new course content group

Creates a new course content group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_content_group_create_dto: OpenapiClient::CourseContentGroupCreateDto.new({name: 'name_example', course_id: 'course_id_example'}) # CourseContentGroupCreateDto | 
}

begin
  # Create a new course content group
  api_instance.create_course_content_group_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->create_course_content_group_async: #{e}"
end
```

#### Using the create_course_content_group_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_content_group_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course content group
  data, status_code, headers = api_instance.create_course_content_group_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->create_course_content_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_content_group_create_dto** | [**CourseContentGroupCreateDto**](CourseContentGroupCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_content_group_async

> delete_course_content_group_async(tenant_id, group_id, opts)

Delete a course content group

Deletes a course content group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
group_id = 'group_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course content group
  api_instance.delete_course_content_group_async(tenant_id, group_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->delete_course_content_group_async: #{e}"
end
```

#### Using the delete_course_content_group_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_content_group_async_with_http_info(tenant_id, group_id, opts)

```ruby
begin
  # Delete a course content group
  data, status_code, headers = api_instance.delete_course_content_group_async_with_http_info(tenant_id, group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->delete_course_content_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_content_group_by_id_async

> <CourseContentGroupDto> get_course_content_group_by_id_async(group_id, opts)

Get course content group by ID

Retrieves a specific course content group by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
group_id = 'group_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course content group by ID
  result = api_instance.get_course_content_group_by_id_async(group_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_group_by_id_async: #{e}"
end
```

#### Using the get_course_content_group_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseContentGroupDto>, Integer, Hash)> get_course_content_group_by_id_async_with_http_info(group_id, opts)

```ruby
begin
  # Get course content group by ID
  data, status_code, headers = api_instance.get_course_content_group_by_id_async_with_http_info(group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseContentGroupDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_group_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseContentGroupDto**](CourseContentGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_content_groups_async

> <Array<CourseContentGroupDto>> get_course_content_groups_async(tenant_id, opts)

Get all course content groups

Retrieves all course content groups for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course content groups
  result = api_instance.get_course_content_groups_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_async: #{e}"
end
```

#### Using the get_course_content_groups_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseContentGroupDto>>, Integer, Hash)> get_course_content_groups_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course content groups
  data, status_code, headers = api_instance.get_course_content_groups_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseContentGroupDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseContentGroupDto&gt;**](CourseContentGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_content_groups_by_course_async

> <Array<CourseContentGroupDto>> get_course_content_groups_by_course_async(course_id, opts)

Get course content groups by course

Retrieves all course content groups for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course content groups by course
  result = api_instance.get_course_content_groups_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_by_course_async: #{e}"
end
```

#### Using the get_course_content_groups_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseContentGroupDto>>, Integer, Hash)> get_course_content_groups_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course content groups by course
  data, status_code, headers = api_instance.get_course_content_groups_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseContentGroupDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseContentGroupDto&gt;**](CourseContentGroupDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_content_groups_by_course_count_async

> Integer get_course_content_groups_by_course_count_async(course_id, opts)

Get course content groups count by course

Returns the count of course content groups for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course content groups count by course
  result = api_instance.get_course_content_groups_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_by_course_count_async: #{e}"
end
```

#### Using the get_course_content_groups_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_content_groups_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course content groups count by course
  data, status_code, headers = api_instance.get_course_content_groups_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_by_course_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_content_groups_count_async

> Integer get_course_content_groups_count_async(tenant_id, opts)

Get course content groups count

Returns the count of course content groups for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course content groups count
  result = api_instance.get_course_content_groups_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_count_async: #{e}"
end
```

#### Using the get_course_content_groups_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_content_groups_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course content groups count
  data, status_code, headers = api_instance.get_course_content_groups_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->get_course_content_groups_count_async_with_http_info: #{e}"
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


## update_course_content_group_async

> update_course_content_group_async(tenant_id, group_id, opts)

Update a course content group

Updates an existing course content group for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseContentGroupsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
group_id = 'group_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_content_group_update_dto: OpenapiClient::CourseContentGroupUpdateDto.new # CourseContentGroupUpdateDto | 
}

begin
  # Update a course content group
  api_instance.update_course_content_group_async(tenant_id, group_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->update_course_content_group_async: #{e}"
end
```

#### Using the update_course_content_group_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_content_group_async_with_http_info(tenant_id, group_id, opts)

```ruby
begin
  # Update a course content group
  data, status_code, headers = api_instance.update_course_content_group_async_with_http_info(tenant_id, group_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseContentGroupsApi->update_course_content_group_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **group_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_content_group_update_dto** | [**CourseContentGroupUpdateDto**](CourseContentGroupUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

