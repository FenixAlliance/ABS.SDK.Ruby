# OpenapiClient::CourseEnrollmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_enrollment_async**](CourseEnrollmentsApi.md#create_course_enrollment_async) | **POST** /api/v2/LearningService/CourseEnrollments | Create a new course enrollment |
| [**delete_course_enrollment_async**](CourseEnrollmentsApi.md#delete_course_enrollment_async) | **DELETE** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Delete a course enrollment |
| [**get_course_enrollment_async**](CourseEnrollmentsApi.md#get_course_enrollment_async) | **GET** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Get course enrollment by ID |
| [**get_enrollments_async**](CourseEnrollmentsApi.md#get_enrollments_async) | **GET** /api/v2/LearningService/CourseEnrollments | Get all course enrollments |
| [**get_enrollments_count_async**](CourseEnrollmentsApi.md#get_enrollments_count_async) | **GET** /api/v2/LearningService/CourseEnrollments/Count | Get course enrollments count |
| [**get_student_course_enrollments_async**](CourseEnrollmentsApi.md#get_student_course_enrollments_async) | **GET** /api/v2/LearningService/CourseEnrollments/Student/{studentProfileId} | Get enrollments by student |
| [**patch_course_enrollment_async**](CourseEnrollmentsApi.md#patch_course_enrollment_async) | **PATCH** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Patch a course enrollment |
| [**update_course_enrollment_async**](CourseEnrollmentsApi.md#update_course_enrollment_async) | **PUT** /api/v2/LearningService/CourseEnrollments/{courseEnrollmentId} | Update a course enrollment |


## create_course_enrollment_async

> create_course_enrollment_async(tenant_id, opts)

Create a new course enrollment

Creates a new course enrollment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_enrollment_create_dto: OpenapiClient::CourseEnrollmentCreateDto.new # CourseEnrollmentCreateDto | 
}

begin
  # Create a new course enrollment
  api_instance.create_course_enrollment_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->create_course_enrollment_async: #{e}"
end
```

#### Using the create_course_enrollment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_enrollment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course enrollment
  data, status_code, headers = api_instance.create_course_enrollment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->create_course_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_enrollment_create_dto** | [**CourseEnrollmentCreateDto**](CourseEnrollmentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_enrollment_async

> delete_course_enrollment_async(tenant_id, course_enrollment_id, opts)

Delete a course enrollment

Deletes a course enrollment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course enrollment
  api_instance.delete_course_enrollment_async(tenant_id, course_enrollment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->delete_course_enrollment_async: #{e}"
end
```

#### Using the delete_course_enrollment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)

```ruby
begin
  # Delete a course enrollment
  data, status_code, headers = api_instance.delete_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->delete_course_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_enrollment_async

> <CourseEnrollmentDto> get_course_enrollment_async(tenant_id, course_enrollment_id, opts)

Get course enrollment by ID

Retrieves a specific course enrollment by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course enrollment by ID
  result = api_instance.get_course_enrollment_async(tenant_id, course_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_course_enrollment_async: #{e}"
end
```

#### Using the get_course_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseEnrollmentDto>, Integer, Hash)> get_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)

```ruby
begin
  # Get course enrollment by ID
  data, status_code, headers = api_instance.get_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseEnrollmentDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_course_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseEnrollmentDto**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollments_async

> <Array<CourseEnrollmentDto>> get_enrollments_async(tenant_id, opts)

Get all course enrollments

Retrieves all course enrollments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course enrollments
  result = api_instance.get_enrollments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_enrollments_async: #{e}"
end
```

#### Using the get_enrollments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseEnrollmentDto>>, Integer, Hash)> get_enrollments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course enrollments
  data, status_code, headers = api_instance.get_enrollments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseEnrollmentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_enrollments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseEnrollmentDto&gt;**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollments_count_async

> Integer get_enrollments_count_async(tenant_id, opts)

Get course enrollments count

Returns the count of course enrollments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course enrollments count
  result = api_instance.get_enrollments_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_enrollments_count_async: #{e}"
end
```

#### Using the get_enrollments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_enrollments_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course enrollments count
  data, status_code, headers = api_instance.get_enrollments_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_enrollments_count_async_with_http_info: #{e}"
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


## get_student_course_enrollments_async

> <Array<CourseEnrollmentDto>> get_student_course_enrollments_async(tenant_id, student_profile_id, opts)

Get enrollments by student

Retrieves all enrollments for a specific student.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
student_profile_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get enrollments by student
  result = api_instance.get_student_course_enrollments_async(tenant_id, student_profile_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_student_course_enrollments_async: #{e}"
end
```

#### Using the get_student_course_enrollments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseEnrollmentDto>>, Integer, Hash)> get_student_course_enrollments_async_with_http_info(tenant_id, student_profile_id, opts)

```ruby
begin
  # Get enrollments by student
  data, status_code, headers = api_instance.get_student_course_enrollments_async_with_http_info(tenant_id, student_profile_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseEnrollmentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->get_student_course_enrollments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **student_profile_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseEnrollmentDto&gt;**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_course_enrollment_async

> patch_course_enrollment_async(tenant_id, course_enrollment_id, opts)

Patch a course enrollment

Partially updates an existing course enrollment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course enrollment
  api_instance.patch_course_enrollment_async(tenant_id, course_enrollment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->patch_course_enrollment_async: #{e}"
end
```

#### Using the patch_course_enrollment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)

```ruby
begin
  # Patch a course enrollment
  data, status_code, headers = api_instance.patch_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->patch_course_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_enrollment_id** | **String** |  |  |
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


## update_course_enrollment_async

> update_course_enrollment_async(tenant_id, course_enrollment_id, opts)

Update a course enrollment

Updates an existing course enrollment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_enrollment_update_dto: OpenapiClient::CourseEnrollmentUpdateDto.new # CourseEnrollmentUpdateDto | 
}

begin
  # Update a course enrollment
  api_instance.update_course_enrollment_async(tenant_id, course_enrollment_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->update_course_enrollment_async: #{e}"
end
```

#### Using the update_course_enrollment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)

```ruby
begin
  # Update a course enrollment
  data, status_code, headers = api_instance.update_course_enrollment_async_with_http_info(tenant_id, course_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseEnrollmentsApi->update_course_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_enrollment_update_dto** | [**CourseEnrollmentUpdateDto**](CourseEnrollmentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

