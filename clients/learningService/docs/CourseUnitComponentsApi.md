# OpenapiClient::CourseUnitComponentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_unit_component_async**](CourseUnitComponentsApi.md#create_course_unit_component_async) | **POST** /api/v2/LearningService/CourseUnitComponents | Create a new course unit component |
| [**delete_course_unit_component_async**](CourseUnitComponentsApi.md#delete_course_unit_component_async) | **DELETE** /api/v2/LearningService/CourseUnitComponents/{componentId} | Delete a course unit component |
| [**get_course_unit_component_by_id_async**](CourseUnitComponentsApi.md#get_course_unit_component_by_id_async) | **GET** /api/v2/LearningService/CourseUnitComponents/{componentId} | Get course unit component by ID |
| [**get_course_unit_components_async**](CourseUnitComponentsApi.md#get_course_unit_components_async) | **GET** /api/v2/LearningService/CourseUnitComponents | Get all course unit components |
| [**get_course_unit_components_count_async**](CourseUnitComponentsApi.md#get_course_unit_components_count_async) | **GET** /api/v2/LearningService/CourseUnitComponents/Count | Get course unit components count |
| [**patch_course_unit_component_async**](CourseUnitComponentsApi.md#patch_course_unit_component_async) | **PATCH** /api/v2/LearningService/CourseUnitComponents/{componentId} | Patch a course unit component |
| [**update_course_unit_component_async**](CourseUnitComponentsApi.md#update_course_unit_component_async) | **PUT** /api/v2/LearningService/CourseUnitComponents/{componentId} | Update a course unit component |


## create_course_unit_component_async

> create_course_unit_component_async(tenant_id, opts)

Create a new course unit component

Creates a new course unit component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_unit_component_create_dto: OpenapiClient::CourseUnitComponentCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CourseUnitComponentCreateDto | 
}

begin
  # Create a new course unit component
  api_instance.create_course_unit_component_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->create_course_unit_component_async: #{e}"
end
```

#### Using the create_course_unit_component_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_unit_component_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course unit component
  data, status_code, headers = api_instance.create_course_unit_component_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->create_course_unit_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_unit_component_create_dto** | [**CourseUnitComponentCreateDto**](CourseUnitComponentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_unit_component_async

> delete_course_unit_component_async(tenant_id, component_id, opts)

Delete a course unit component

Deletes a course unit component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
component_id = 'component_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course unit component
  api_instance.delete_course_unit_component_async(tenant_id, component_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->delete_course_unit_component_async: #{e}"
end
```

#### Using the delete_course_unit_component_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_unit_component_async_with_http_info(tenant_id, component_id, opts)

```ruby
begin
  # Delete a course unit component
  data, status_code, headers = api_instance.delete_course_unit_component_async_with_http_info(tenant_id, component_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->delete_course_unit_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **component_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_unit_component_by_id_async

> <CourseUnitComponentDto> get_course_unit_component_by_id_async(component_id, opts)

Get course unit component by ID

Retrieves a specific course unit component by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
component_id = 'component_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course unit component by ID
  result = api_instance.get_course_unit_component_by_id_async(component_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->get_course_unit_component_by_id_async: #{e}"
end
```

#### Using the get_course_unit_component_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseUnitComponentDto>, Integer, Hash)> get_course_unit_component_by_id_async_with_http_info(component_id, opts)

```ruby
begin
  # Get course unit component by ID
  data, status_code, headers = api_instance.get_course_unit_component_by_id_async_with_http_info(component_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseUnitComponentDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->get_course_unit_component_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **component_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseUnitComponentDto**](CourseUnitComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_unit_components_async

> <Array<CourseUnitComponentDto>> get_course_unit_components_async(tenant_id, opts)

Get all course unit components

Retrieves all course unit components for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course unit components
  result = api_instance.get_course_unit_components_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->get_course_unit_components_async: #{e}"
end
```

#### Using the get_course_unit_components_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseUnitComponentDto>>, Integer, Hash)> get_course_unit_components_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course unit components
  data, status_code, headers = api_instance.get_course_unit_components_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseUnitComponentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->get_course_unit_components_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseUnitComponentDto&gt;**](CourseUnitComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_unit_components_count_async

> Integer get_course_unit_components_count_async(tenant_id, opts)

Get course unit components count

Returns the count of course unit components for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course unit components count
  result = api_instance.get_course_unit_components_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->get_course_unit_components_count_async: #{e}"
end
```

#### Using the get_course_unit_components_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_unit_components_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course unit components count
  data, status_code, headers = api_instance.get_course_unit_components_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->get_course_unit_components_count_async_with_http_info: #{e}"
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


## patch_course_unit_component_async

> <EmptyEnvelope> patch_course_unit_component_async(tenant_id, component_id, opts)

Patch a course unit component

Partially updates a course unit component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
component_id = 'component_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course unit component
  result = api_instance.patch_course_unit_component_async(tenant_id, component_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->patch_course_unit_component_async: #{e}"
end
```

#### Using the patch_course_unit_component_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_unit_component_async_with_http_info(tenant_id, component_id, opts)

```ruby
begin
  # Patch a course unit component
  data, status_code, headers = api_instance.patch_course_unit_component_async_with_http_info(tenant_id, component_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->patch_course_unit_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **component_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_course_unit_component_async

> update_course_unit_component_async(tenant_id, component_id, opts)

Update a course unit component

Updates an existing course unit component for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseUnitComponentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
component_id = 'component_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_unit_component_update_dto: OpenapiClient::CourseUnitComponentUpdateDto.new # CourseUnitComponentUpdateDto | 
}

begin
  # Update a course unit component
  api_instance.update_course_unit_component_async(tenant_id, component_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->update_course_unit_component_async: #{e}"
end
```

#### Using the update_course_unit_component_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_unit_component_async_with_http_info(tenant_id, component_id, opts)

```ruby
begin
  # Update a course unit component
  data, status_code, headers = api_instance.update_course_unit_component_async_with_http_info(tenant_id, component_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseUnitComponentsApi->update_course_unit_component_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **component_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_unit_component_update_dto** | [**CourseUnitComponentUpdateDto**](CourseUnitComponentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

