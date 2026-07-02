# OpenapiClient::CourseSectionsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_section_async**](CourseSectionsApi.md#create_course_section_async) | **POST** /api/v2/LearningService/CourseSections | Create a new course section |
| [**delete_course_section_async**](CourseSectionsApi.md#delete_course_section_async) | **DELETE** /api/v2/LearningService/CourseSections/{sectionId} | Delete a course section |
| [**get_course_section_by_id_async**](CourseSectionsApi.md#get_course_section_by_id_async) | **GET** /api/v2/LearningService/CourseSections/{sectionId} | Get course section by ID |
| [**get_course_sections_async**](CourseSectionsApi.md#get_course_sections_async) | **GET** /api/v2/LearningService/CourseSections | Get all course sections |
| [**get_course_sections_count_async**](CourseSectionsApi.md#get_course_sections_count_async) | **GET** /api/v2/LearningService/CourseSections/Count | Get course sections count |
| [**patch_course_section_async**](CourseSectionsApi.md#patch_course_section_async) | **PATCH** /api/v2/LearningService/CourseSections/{sectionId} | Patch a course section |
| [**update_course_section_async**](CourseSectionsApi.md#update_course_section_async) | **PUT** /api/v2/LearningService/CourseSections/{sectionId} | Update a course section |


## create_course_section_async

> create_course_section_async(tenant_id, opts)

Create a new course section

Creates a new course section for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_section_create_dto: OpenapiClient::CourseSectionCreateDto.new({name: 'name_example', course_id: 'course_id_example'}) # CourseSectionCreateDto | 
}

begin
  # Create a new course section
  api_instance.create_course_section_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->create_course_section_async: #{e}"
end
```

#### Using the create_course_section_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_section_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course section
  data, status_code, headers = api_instance.create_course_section_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->create_course_section_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_section_create_dto** | [**CourseSectionCreateDto**](CourseSectionCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_section_async

> delete_course_section_async(tenant_id, section_id, opts)

Delete a course section

Deletes a course section for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
section_id = 'section_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course section
  api_instance.delete_course_section_async(tenant_id, section_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->delete_course_section_async: #{e}"
end
```

#### Using the delete_course_section_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_section_async_with_http_info(tenant_id, section_id, opts)

```ruby
begin
  # Delete a course section
  data, status_code, headers = api_instance.delete_course_section_async_with_http_info(tenant_id, section_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->delete_course_section_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **section_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_section_by_id_async

> <CourseSectionDto> get_course_section_by_id_async(section_id, opts)

Get course section by ID

Retrieves a specific course section by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
section_id = 'section_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course section by ID
  result = api_instance.get_course_section_by_id_async(section_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->get_course_section_by_id_async: #{e}"
end
```

#### Using the get_course_section_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseSectionDto>, Integer, Hash)> get_course_section_by_id_async_with_http_info(section_id, opts)

```ruby
begin
  # Get course section by ID
  data, status_code, headers = api_instance.get_course_section_by_id_async_with_http_info(section_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseSectionDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->get_course_section_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **section_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseSectionDto**](CourseSectionDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_sections_async

> <Array<CourseSectionDto>> get_course_sections_async(tenant_id, opts)

Get all course sections

Retrieves all course sections for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course sections
  result = api_instance.get_course_sections_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->get_course_sections_async: #{e}"
end
```

#### Using the get_course_sections_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseSectionDto>>, Integer, Hash)> get_course_sections_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course sections
  data, status_code, headers = api_instance.get_course_sections_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseSectionDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->get_course_sections_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseSectionDto&gt;**](CourseSectionDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_sections_count_async

> Integer get_course_sections_count_async(tenant_id, opts)

Get course sections count

Returns the count of course sections for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course sections count
  result = api_instance.get_course_sections_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->get_course_sections_count_async: #{e}"
end
```

#### Using the get_course_sections_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_sections_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course sections count
  data, status_code, headers = api_instance.get_course_sections_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->get_course_sections_count_async_with_http_info: #{e}"
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


## patch_course_section_async

> <EmptyEnvelope> patch_course_section_async(tenant_id, section_id, opts)

Patch a course section

Partially updates a course section for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
section_id = 'section_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course section
  result = api_instance.patch_course_section_async(tenant_id, section_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->patch_course_section_async: #{e}"
end
```

#### Using the patch_course_section_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_section_async_with_http_info(tenant_id, section_id, opts)

```ruby
begin
  # Patch a course section
  data, status_code, headers = api_instance.patch_course_section_async_with_http_info(tenant_id, section_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->patch_course_section_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **section_id** | **String** |  |  |
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


## update_course_section_async

> update_course_section_async(tenant_id, section_id, opts)

Update a course section

Updates an existing course section for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseSectionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
section_id = 'section_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_section_update_dto: OpenapiClient::CourseSectionUpdateDto.new # CourseSectionUpdateDto | 
}

begin
  # Update a course section
  api_instance.update_course_section_async(tenant_id, section_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->update_course_section_async: #{e}"
end
```

#### Using the update_course_section_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_section_async_with_http_info(tenant_id, section_id, opts)

```ruby
begin
  # Update a course section
  data, status_code, headers = api_instance.update_course_section_async_with_http_info(tenant_id, section_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseSectionsApi->update_course_section_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **section_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_section_update_dto** | [**CourseSectionUpdateDto**](CourseSectionUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

