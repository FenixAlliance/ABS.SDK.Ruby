# OpenapiClient::CourseGradingRubricsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_grading_rubric_async**](CourseGradingRubricsApi.md#create_course_grading_rubric_async) | **POST** /api/v2/LearningService/CourseGradingRubrics | Create a course grading rubric |
| [**delete_course_grading_rubric_async**](CourseGradingRubricsApi.md#delete_course_grading_rubric_async) | **DELETE** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Delete a course grading rubric |
| [**get_course_grading_rubric_by_id_async**](CourseGradingRubricsApi.md#get_course_grading_rubric_by_id_async) | **GET** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Get course grading rubric by ID |
| [**get_course_grading_rubrics_async**](CourseGradingRubricsApi.md#get_course_grading_rubrics_async) | **GET** /api/v2/LearningService/CourseGradingRubrics | Get all course grading rubrics |
| [**get_course_grading_rubrics_count_async**](CourseGradingRubricsApi.md#get_course_grading_rubrics_count_async) | **GET** /api/v2/LearningService/CourseGradingRubrics/Count | Get course grading rubrics count |
| [**patch_course_grading_rubric_async**](CourseGradingRubricsApi.md#patch_course_grading_rubric_async) | **PATCH** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Patch a course grading rubric |
| [**update_course_grading_rubric_async**](CourseGradingRubricsApi.md#update_course_grading_rubric_async) | **PUT** /api/v2/LearningService/CourseGradingRubrics/{rubricId} | Update a course grading rubric |


## create_course_grading_rubric_async

> create_course_grading_rubric_async(tenant_id, opts)

Create a course grading rubric

Creates a new course grading rubric for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_grading_rubric_create_dto: OpenapiClient::CourseGradingRubricCreateDto.new({title: 'title_example', course_id: 'course_id_example'}) # CourseGradingRubricCreateDto | 
}

begin
  # Create a course grading rubric
  api_instance.create_course_grading_rubric_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->create_course_grading_rubric_async: #{e}"
end
```

#### Using the create_course_grading_rubric_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_grading_rubric_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course grading rubric
  data, status_code, headers = api_instance.create_course_grading_rubric_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->create_course_grading_rubric_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_grading_rubric_create_dto** | [**CourseGradingRubricCreateDto**](CourseGradingRubricCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_grading_rubric_async

> delete_course_grading_rubric_async(tenant_id, rubric_id, opts)

Delete a course grading rubric

Deletes a course grading rubric by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rubric_id = 'rubric_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course grading rubric
  api_instance.delete_course_grading_rubric_async(tenant_id, rubric_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->delete_course_grading_rubric_async: #{e}"
end
```

#### Using the delete_course_grading_rubric_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_grading_rubric_async_with_http_info(tenant_id, rubric_id, opts)

```ruby
begin
  # Delete a course grading rubric
  data, status_code, headers = api_instance.delete_course_grading_rubric_async_with_http_info(tenant_id, rubric_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->delete_course_grading_rubric_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rubric_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_grading_rubric_by_id_async

> <CourseGradingRubricDto> get_course_grading_rubric_by_id_async(rubric_id, opts)

Get course grading rubric by ID

Retrieves a specific course grading rubric by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
rubric_id = 'rubric_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course grading rubric by ID
  result = api_instance.get_course_grading_rubric_by_id_async(rubric_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->get_course_grading_rubric_by_id_async: #{e}"
end
```

#### Using the get_course_grading_rubric_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseGradingRubricDto>, Integer, Hash)> get_course_grading_rubric_by_id_async_with_http_info(rubric_id, opts)

```ruby
begin
  # Get course grading rubric by ID
  data, status_code, headers = api_instance.get_course_grading_rubric_by_id_async_with_http_info(rubric_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseGradingRubricDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->get_course_grading_rubric_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **rubric_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseGradingRubricDto**](CourseGradingRubricDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_grading_rubrics_async

> <Array<CourseGradingRubricDto>> get_course_grading_rubrics_async(tenant_id, opts)

Get all course grading rubrics

Retrieves all course grading rubrics for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course grading rubrics
  result = api_instance.get_course_grading_rubrics_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->get_course_grading_rubrics_async: #{e}"
end
```

#### Using the get_course_grading_rubrics_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseGradingRubricDto>>, Integer, Hash)> get_course_grading_rubrics_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course grading rubrics
  data, status_code, headers = api_instance.get_course_grading_rubrics_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseGradingRubricDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->get_course_grading_rubrics_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseGradingRubricDto&gt;**](CourseGradingRubricDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_grading_rubrics_count_async

> Integer get_course_grading_rubrics_count_async(tenant_id, opts)

Get course grading rubrics count

Returns the count of course grading rubrics for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course grading rubrics count
  result = api_instance.get_course_grading_rubrics_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->get_course_grading_rubrics_count_async: #{e}"
end
```

#### Using the get_course_grading_rubrics_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_grading_rubrics_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course grading rubrics count
  data, status_code, headers = api_instance.get_course_grading_rubrics_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->get_course_grading_rubrics_count_async_with_http_info: #{e}"
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


## patch_course_grading_rubric_async

> patch_course_grading_rubric_async(tenant_id, rubric_id, opts)

Patch a course grading rubric

Partially updates an existing course grading rubric.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rubric_id = 'rubric_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course grading rubric
  api_instance.patch_course_grading_rubric_async(tenant_id, rubric_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->patch_course_grading_rubric_async: #{e}"
end
```

#### Using the patch_course_grading_rubric_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_course_grading_rubric_async_with_http_info(tenant_id, rubric_id, opts)

```ruby
begin
  # Patch a course grading rubric
  data, status_code, headers = api_instance.patch_course_grading_rubric_async_with_http_info(tenant_id, rubric_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->patch_course_grading_rubric_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rubric_id** | **String** |  |  |
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


## update_course_grading_rubric_async

> update_course_grading_rubric_async(tenant_id, rubric_id, opts)

Update a course grading rubric

Updates an existing course grading rubric.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseGradingRubricsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
rubric_id = 'rubric_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_grading_rubric_update_dto: OpenapiClient::CourseGradingRubricUpdateDto.new # CourseGradingRubricUpdateDto | 
}

begin
  # Update a course grading rubric
  api_instance.update_course_grading_rubric_async(tenant_id, rubric_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->update_course_grading_rubric_async: #{e}"
end
```

#### Using the update_course_grading_rubric_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_grading_rubric_async_with_http_info(tenant_id, rubric_id, opts)

```ruby
begin
  # Update a course grading rubric
  data, status_code, headers = api_instance.update_course_grading_rubric_async_with_http_info(tenant_id, rubric_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseGradingRubricsApi->update_course_grading_rubric_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **rubric_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_grading_rubric_update_dto** | [**CourseGradingRubricUpdateDto**](CourseGradingRubricUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

