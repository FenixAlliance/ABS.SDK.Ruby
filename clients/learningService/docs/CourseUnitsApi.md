# OpenapiClient::CourseUnitsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_unit_async**](CourseUnitsApi.md#create_course_unit_async) | **POST** /api/v2/LearningService/CourseUnits | Create a new course unit |
| [**delete_course_unit_async**](CourseUnitsApi.md#delete_course_unit_async) | **DELETE** /api/v2/LearningService/CourseUnits/{unitId} | Delete a course unit |
| [**get_course_unit_by_id_async**](CourseUnitsApi.md#get_course_unit_by_id_async) | **GET** /api/v2/LearningService/CourseUnits/{unitId} | Get course unit by ID |
| [**get_course_units_async**](CourseUnitsApi.md#get_course_units_async) | **GET** /api/v2/LearningService/CourseUnits | Get all course units |
| [**get_course_units_count_async**](CourseUnitsApi.md#get_course_units_count_async) | **GET** /api/v2/LearningService/CourseUnits/Count | Get course units count |
| [**update_course_unit_async**](CourseUnitsApi.md#update_course_unit_async) | **PUT** /api/v2/LearningService/CourseUnits/{unitId} | Update a course unit |


## create_course_unit_async

> create_course_unit_async(tenant_id, opts)

Create a new course unit

Creates a new course unit for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_unit_create_dto: OpenapiClient::CourseUnitCreateDto.new({title: 'title_example', course_id: 'course_id_example', course_section_id: 'course_section_id_example'}) # CourseUnitCreateDto | 
}

begin
  # Create a new course unit
  api_instance.create_course_unit_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->create_course_unit_async: #{e}"
end
```

#### Using the create_course_unit_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_unit_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course unit
  data, status_code, headers = api_instance.create_course_unit_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->create_course_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_unit_create_dto** | [**CourseUnitCreateDto**](CourseUnitCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_unit_async

> delete_course_unit_async(tenant_id, unit_id, opts)

Delete a course unit

Deletes a course unit for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_id = 'unit_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course unit
  api_instance.delete_course_unit_async(tenant_id, unit_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->delete_course_unit_async: #{e}"
end
```

#### Using the delete_course_unit_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_unit_async_with_http_info(tenant_id, unit_id, opts)

```ruby
begin
  # Delete a course unit
  data, status_code, headers = api_instance.delete_course_unit_async_with_http_info(tenant_id, unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->delete_course_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_unit_by_id_async

> <CourseUnitDto> get_course_unit_by_id_async(unit_id, opts)

Get course unit by ID

Retrieves a specific course unit by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitsApi.new
unit_id = 'unit_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course unit by ID
  result = api_instance.get_course_unit_by_id_async(unit_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->get_course_unit_by_id_async: #{e}"
end
```

#### Using the get_course_unit_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseUnitDto>, Integer, Hash)> get_course_unit_by_id_async_with_http_info(unit_id, opts)

```ruby
begin
  # Get course unit by ID
  data, status_code, headers = api_instance.get_course_unit_by_id_async_with_http_info(unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseUnitDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->get_course_unit_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseUnitDto**](CourseUnitDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_units_async

> <Array<CourseUnitDto>> get_course_units_async(tenant_id, opts)

Get all course units

Retrieves all course units for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course units
  result = api_instance.get_course_units_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->get_course_units_async: #{e}"
end
```

#### Using the get_course_units_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseUnitDto>>, Integer, Hash)> get_course_units_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course units
  data, status_code, headers = api_instance.get_course_units_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseUnitDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->get_course_units_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseUnitDto&gt;**](CourseUnitDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_units_count_async

> Integer get_course_units_count_async(tenant_id, opts)

Get course units count

Returns the count of course units for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course units count
  result = api_instance.get_course_units_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->get_course_units_count_async: #{e}"
end
```

#### Using the get_course_units_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_units_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course units count
  data, status_code, headers = api_instance.get_course_units_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->get_course_units_count_async_with_http_info: #{e}"
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


## update_course_unit_async

> update_course_unit_async(tenant_id, unit_id, opts)

Update a course unit

Updates an existing course unit for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
unit_id = 'unit_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_unit_update_dto: OpenapiClient::CourseUnitUpdateDto.new # CourseUnitUpdateDto | 
}

begin
  # Update a course unit
  api_instance.update_course_unit_async(tenant_id, unit_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->update_course_unit_async: #{e}"
end
```

#### Using the update_course_unit_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_unit_async_with_http_info(tenant_id, unit_id, opts)

```ruby
begin
  # Update a course unit
  data, status_code, headers = api_instance.update_course_unit_async_with_http_info(tenant_id, unit_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitsApi->update_course_unit_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **unit_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_unit_update_dto** | [**CourseUnitUpdateDto**](CourseUnitUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

