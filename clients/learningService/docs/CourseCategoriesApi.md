# OpenapiClient::CourseCategoriesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_category_async**](CourseCategoriesApi.md#create_course_category_async) | **POST** /api/v2/LearningService/CourseCategories | Create a new course category |
| [**delete_course_category_async**](CourseCategoriesApi.md#delete_course_category_async) | **DELETE** /api/v2/LearningService/CourseCategories/{categoryId} | Delete a course category |
| [**get_course_categories_async**](CourseCategoriesApi.md#get_course_categories_async) | **GET** /api/v2/LearningService/CourseCategories | Get all course categories |
| [**get_course_categories_count_async**](CourseCategoriesApi.md#get_course_categories_count_async) | **GET** /api/v2/LearningService/CourseCategories/Count | Get course categories count |
| [**get_course_category_by_id_async**](CourseCategoriesApi.md#get_course_category_by_id_async) | **GET** /api/v2/LearningService/CourseCategories/{categoryId} | Get course category by ID |
| [**update_course_category_async**](CourseCategoriesApi.md#update_course_category_async) | **PUT** /api/v2/LearningService/CourseCategories/{categoryId} | Update a course category |


## create_course_category_async

> create_course_category_async(tenant_id, opts)

Create a new course category

Creates a new course category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_category_create_dto: OpenapiClient::CourseCategoryCreateDto.new({title: 'title_example', business_id: 'business_id_example'}) # CourseCategoryCreateDto | 
}

begin
  # Create a new course category
  api_instance.create_course_category_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->create_course_category_async: #{e}"
end
```

#### Using the create_course_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_category_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course category
  data, status_code, headers = api_instance.create_course_category_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->create_course_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_category_create_dto** | [**CourseCategoryCreateDto**](CourseCategoryCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_category_async

> delete_course_category_async(tenant_id, category_id, opts)

Delete a course category

Deletes a course category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = 'category_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course category
  api_instance.delete_course_category_async(tenant_id, category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->delete_course_category_async: #{e}"
end
```

#### Using the delete_course_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_category_async_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Delete a course category
  data, status_code, headers = api_instance.delete_course_category_async_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->delete_course_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_categories_async

> <Array<CourseCategoryDto>> get_course_categories_async(tenant_id, opts)

Get all course categories

Retrieves all course categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course categories
  result = api_instance.get_course_categories_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->get_course_categories_async: #{e}"
end
```

#### Using the get_course_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseCategoryDto>>, Integer, Hash)> get_course_categories_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course categories
  data, status_code, headers = api_instance.get_course_categories_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseCategoryDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->get_course_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseCategoryDto&gt;**](CourseCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_categories_count_async

> Integer get_course_categories_count_async(tenant_id, opts)

Get course categories count

Returns the count of course categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course categories count
  result = api_instance.get_course_categories_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->get_course_categories_count_async: #{e}"
end
```

#### Using the get_course_categories_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_categories_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course categories count
  data, status_code, headers = api_instance.get_course_categories_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->get_course_categories_count_async_with_http_info: #{e}"
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


## get_course_category_by_id_async

> <CourseCategoryDto> get_course_category_by_id_async(category_id, opts)

Get course category by ID

Retrieves a specific course category by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCategoriesApi.new
category_id = 'category_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course category by ID
  result = api_instance.get_course_category_by_id_async(category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->get_course_category_by_id_async: #{e}"
end
```

#### Using the get_course_category_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseCategoryDto>, Integer, Hash)> get_course_category_by_id_async_with_http_info(category_id, opts)

```ruby
begin
  # Get course category by ID
  data, status_code, headers = api_instance.get_course_category_by_id_async_with_http_info(category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseCategoryDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->get_course_category_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseCategoryDto**](CourseCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_course_category_async

> update_course_category_async(tenant_id, category_id, opts)

Update a course category

Updates an existing course category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = 'category_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_category_update_dto: OpenapiClient::CourseCategoryUpdateDto.new # CourseCategoryUpdateDto | 
}

begin
  # Update a course category
  api_instance.update_course_category_async(tenant_id, category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->update_course_category_async: #{e}"
end
```

#### Using the update_course_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_category_async_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Update a course category
  data, status_code, headers = api_instance.update_course_category_async_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCategoriesApi->update_course_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_category_update_dto** | [**CourseCategoryUpdateDto**](CourseCategoryUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

