# OpenapiClient::CourseCohortsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_cohort_async**](CourseCohortsApi.md#create_course_cohort_async) | **POST** /api/v2/LearningService/CourseCohorts | Create a new course cohort |
| [**delete_course_cohort_async**](CourseCohortsApi.md#delete_course_cohort_async) | **DELETE** /api/v2/LearningService/CourseCohorts/{cohortId} | Delete a course cohort |
| [**get_course_cohort_by_id_async**](CourseCohortsApi.md#get_course_cohort_by_id_async) | **GET** /api/v2/LearningService/CourseCohorts/{cohortId} | Get course cohort by ID |
| [**get_course_cohorts_async**](CourseCohortsApi.md#get_course_cohorts_async) | **GET** /api/v2/LearningService/CourseCohorts | Get all course cohorts |
| [**get_course_cohorts_count_async**](CourseCohortsApi.md#get_course_cohorts_count_async) | **GET** /api/v2/LearningService/CourseCohorts/Count | Get course cohorts count |
| [**patch_course_cohort_async**](CourseCohortsApi.md#patch_course_cohort_async) | **PATCH** /api/v2/LearningService/CourseCohorts/{cohortId} | Patch a course cohort |
| [**update_course_cohort_async**](CourseCohortsApi.md#update_course_cohort_async) | **PUT** /api/v2/LearningService/CourseCohorts/{cohortId} | Update a course cohort |


## create_course_cohort_async

> create_course_cohort_async(tenant_id, opts)

Create a new course cohort

Creates a new course cohort for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_cohort_create_dto: OpenapiClient::CourseCohortCreateDto.new({name: 'name_example', course_id: 'course_id_example'}) # CourseCohortCreateDto | 
}

begin
  # Create a new course cohort
  api_instance.create_course_cohort_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->create_course_cohort_async: #{e}"
end
```

#### Using the create_course_cohort_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_cohort_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course cohort
  data, status_code, headers = api_instance.create_course_cohort_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->create_course_cohort_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_cohort_create_dto** | [**CourseCohortCreateDto**](CourseCohortCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_cohort_async

> delete_course_cohort_async(tenant_id, cohort_id, opts)

Delete a course cohort

Deletes a course cohort for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cohort_id = 'cohort_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course cohort
  api_instance.delete_course_cohort_async(tenant_id, cohort_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->delete_course_cohort_async: #{e}"
end
```

#### Using the delete_course_cohort_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_cohort_async_with_http_info(tenant_id, cohort_id, opts)

```ruby
begin
  # Delete a course cohort
  data, status_code, headers = api_instance.delete_course_cohort_async_with_http_info(tenant_id, cohort_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->delete_course_cohort_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cohort_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_cohort_by_id_async

> <CourseCohortDto> get_course_cohort_by_id_async(cohort_id, opts)

Get course cohort by ID

Retrieves a specific course cohort by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
cohort_id = 'cohort_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course cohort by ID
  result = api_instance.get_course_cohort_by_id_async(cohort_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->get_course_cohort_by_id_async: #{e}"
end
```

#### Using the get_course_cohort_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseCohortDto>, Integer, Hash)> get_course_cohort_by_id_async_with_http_info(cohort_id, opts)

```ruby
begin
  # Get course cohort by ID
  data, status_code, headers = api_instance.get_course_cohort_by_id_async_with_http_info(cohort_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseCohortDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->get_course_cohort_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cohort_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseCohortDto**](CourseCohortDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_cohorts_async

> <Array<CourseCohortDto>> get_course_cohorts_async(tenant_id, opts)

Get all course cohorts

Retrieves all course cohorts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_cohort_dto_collection_query_parameters: OpenapiClient::CourseCohortDtoCollectionQueryParameters.new # CourseCohortDtoCollectionQueryParameters | 
}

begin
  # Get all course cohorts
  result = api_instance.get_course_cohorts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->get_course_cohorts_async: #{e}"
end
```

#### Using the get_course_cohorts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseCohortDto>>, Integer, Hash)> get_course_cohorts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course cohorts
  data, status_code, headers = api_instance.get_course_cohorts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseCohortDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->get_course_cohorts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_cohort_dto_collection_query_parameters** | [**CourseCohortDtoCollectionQueryParameters**](CourseCohortDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Array&lt;CourseCohortDto&gt;**](CourseCohortDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_course_cohorts_count_async

> Integer get_course_cohorts_count_async(tenant_id, opts)

Get course cohorts count

Returns the count of course cohorts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_cohort_dto_collection_query_parameters: OpenapiClient::CourseCohortDtoCollectionQueryParameters.new # CourseCohortDtoCollectionQueryParameters | 
}

begin
  # Get course cohorts count
  result = api_instance.get_course_cohorts_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->get_course_cohorts_count_async: #{e}"
end
```

#### Using the get_course_cohorts_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_cohorts_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course cohorts count
  data, status_code, headers = api_instance.get_course_cohorts_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->get_course_cohorts_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_cohort_dto_collection_query_parameters** | [**CourseCohortDtoCollectionQueryParameters**](CourseCohortDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_course_cohort_async

> <EmptyEnvelope> patch_course_cohort_async(tenant_id, cohort_id, opts)

Patch a course cohort

Partially updates a course cohort for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cohort_id = 'cohort_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a course cohort
  result = api_instance.patch_course_cohort_async(tenant_id, cohort_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->patch_course_cohort_async: #{e}"
end
```

#### Using the patch_course_cohort_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_cohort_async_with_http_info(tenant_id, cohort_id, opts)

```ruby
begin
  # Patch a course cohort
  data, status_code, headers = api_instance.patch_course_cohort_async_with_http_info(tenant_id, cohort_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->patch_course_cohort_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cohort_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_course_cohort_async

> update_course_cohort_async(tenant_id, cohort_id, opts)

Update a course cohort

Updates an existing course cohort for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCohortsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
cohort_id = 'cohort_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_cohort_update_dto: OpenapiClient::CourseCohortUpdateDto.new # CourseCohortUpdateDto | 
}

begin
  # Update a course cohort
  api_instance.update_course_cohort_async(tenant_id, cohort_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->update_course_cohort_async: #{e}"
end
```

#### Using the update_course_cohort_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_cohort_async_with_http_info(tenant_id, cohort_id, opts)

```ruby
begin
  # Update a course cohort
  data, status_code, headers = api_instance.update_course_cohort_async_with_http_info(tenant_id, cohort_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCohortsApi->update_course_cohort_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **cohort_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_cohort_update_dto** | [**CourseCohortUpdateDto**](CourseCohortUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

