# OpenapiClient::MeApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_my_average_score_async**](MeApi.md#get_my_average_score_async) | **GET** /api/v2/LearningService/Me/AverageScore | Get current user&#39;s average score |
| [**get_my_certificates_async**](MeApi.md#get_my_certificates_async) | **GET** /api/v2/LearningService/Me/Certificates | Get current user&#39;s completion certificates |
| [**get_my_certificates_count_async**](MeApi.md#get_my_certificates_count_async) | **GET** /api/v2/LearningService/Me/Certificates/Count | Get current user&#39;s certificates count |
| [**get_my_enrollments_async**](MeApi.md#get_my_enrollments_async) | **GET** /api/v2/LearningService/Me/Enrollments | Get current user&#39;s course enrollments |
| [**get_my_enrollments_count_async**](MeApi.md#get_my_enrollments_count_async) | **GET** /api/v2/LearningService/Me/Enrollments/Count | Get current user&#39;s enrollment count |
| [**get_my_hours_completed_async**](MeApi.md#get_my_hours_completed_async) | **GET** /api/v2/LearningService/Me/HoursCompleted | Get current user&#39;s completed hours |
| [**get_my_instructor_courses_async**](MeApi.md#get_my_instructor_courses_async) | **GET** /api/v2/LearningService/Me/InstructorCourses | Get current user&#39;s instructor courses |
| [**get_my_instructor_courses_count_async**](MeApi.md#get_my_instructor_courses_count_async) | **GET** /api/v2/LearningService/Me/InstructorCourses/Count | Get current user&#39;s instructor courses count |
| [**get_my_instructor_profiles_async**](MeApi.md#get_my_instructor_profiles_async) | **GET** /api/v2/LearningService/Me/InstructorProfiles | Get current user&#39;s instructor profiles |
| [**get_my_instructor_profiles_count_async**](MeApi.md#get_my_instructor_profiles_count_async) | **GET** /api/v2/LearningService/Me/InstructorProfiles/Count | Get current user&#39;s instructor profiles count |
| [**get_my_pending_task_count_async**](MeApi.md#get_my_pending_task_count_async) | **GET** /api/v2/LearningService/Me/PendingTasks | Get current user&#39;s pending task count |
| [**get_my_student_courses_async**](MeApi.md#get_my_student_courses_async) | **GET** /api/v2/LearningService/Me/Courses | Get current user&#39;s enrolled courses |
| [**get_my_student_courses_count_async**](MeApi.md#get_my_student_courses_count_async) | **GET** /api/v2/LearningService/Me/Courses/Count | Get current user&#39;s enrolled courses count |
| [**get_my_student_profiles_async**](MeApi.md#get_my_student_profiles_async) | **GET** /api/v2/LearningService/Me/StudentProfiles | Get current user&#39;s student profiles |
| [**get_my_student_profiles_count_async**](MeApi.md#get_my_student_profiles_count_async) | **GET** /api/v2/LearningService/Me/StudentProfiles/Count | Get current user&#39;s student profiles count |


## get_my_average_score_async

> <AverageDtoEnvelope> get_my_average_score_async(opts)

Get current user's average score

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's average score
  result = api_instance.get_my_average_score_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_average_score_async: #{e}"
end
```

#### Using the get_my_average_score_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AverageDtoEnvelope>, Integer, Hash)> get_my_average_score_async_with_http_info(opts)

```ruby
begin
  # Get current user's average score
  data, status_code, headers = api_instance.get_my_average_score_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AverageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_average_score_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AverageDtoEnvelope**](AverageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_certificates_async

> <CourseCompletionCertificateDtoIReadOnlyListEnvelope> get_my_certificates_async(opts)

Get current user's completion certificates

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's completion certificates
  result = api_instance.get_my_certificates_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_certificates_async: #{e}"
end
```

#### Using the get_my_certificates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseCompletionCertificateDtoIReadOnlyListEnvelope>, Integer, Hash)> get_my_certificates_async_with_http_info(opts)

```ruby
begin
  # Get current user's completion certificates
  data, status_code, headers = api_instance.get_my_certificates_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseCompletionCertificateDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_certificates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseCompletionCertificateDtoIReadOnlyListEnvelope**](CourseCompletionCertificateDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_certificates_count_async

> Integer get_my_certificates_count_async(opts)

Get current user's certificates count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's certificates count
  result = api_instance.get_my_certificates_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_certificates_count_async: #{e}"
end
```

#### Using the get_my_certificates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_my_certificates_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's certificates count
  data, status_code, headers = api_instance.get_my_certificates_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_certificates_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_enrollments_async

> <CourseEnrollmentDtoIReadOnlyListEnvelope> get_my_enrollments_async(opts)

Get current user's course enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's course enrollments
  result = api_instance.get_my_enrollments_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_enrollments_async: #{e}"
end
```

#### Using the get_my_enrollments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseEnrollmentDtoIReadOnlyListEnvelope>, Integer, Hash)> get_my_enrollments_async_with_http_info(opts)

```ruby
begin
  # Get current user's course enrollments
  data, status_code, headers = api_instance.get_my_enrollments_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseEnrollmentDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_enrollments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseEnrollmentDtoIReadOnlyListEnvelope**](CourseEnrollmentDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_enrollments_count_async

> Integer get_my_enrollments_count_async(opts)

Get current user's enrollment count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's enrollment count
  result = api_instance.get_my_enrollments_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_enrollments_count_async: #{e}"
end
```

#### Using the get_my_enrollments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_my_enrollments_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's enrollment count
  data, status_code, headers = api_instance.get_my_enrollments_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_enrollments_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_hours_completed_async

> <CountDtoEnvelope> get_my_hours_completed_async(opts)

Get current user's completed hours

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's completed hours
  result = api_instance.get_my_hours_completed_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_hours_completed_async: #{e}"
end
```

#### Using the get_my_hours_completed_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountDtoEnvelope>, Integer, Hash)> get_my_hours_completed_async_with_http_info(opts)

```ruby
begin
  # Get current user's completed hours
  data, status_code, headers = api_instance.get_my_hours_completed_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_hours_completed_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountDtoEnvelope**](CountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_instructor_courses_async

> <CourseDtoIReadOnlyListEnvelope> get_my_instructor_courses_async(opts)

Get current user's instructor courses

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's instructor courses
  result = api_instance.get_my_instructor_courses_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_courses_async: #{e}"
end
```

#### Using the get_my_instructor_courses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseDtoIReadOnlyListEnvelope>, Integer, Hash)> get_my_instructor_courses_async_with_http_info(opts)

```ruby
begin
  # Get current user's instructor courses
  data, status_code, headers = api_instance.get_my_instructor_courses_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_courses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseDtoIReadOnlyListEnvelope**](CourseDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_instructor_courses_count_async

> Integer get_my_instructor_courses_count_async(opts)

Get current user's instructor courses count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's instructor courses count
  result = api_instance.get_my_instructor_courses_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_courses_count_async: #{e}"
end
```

#### Using the get_my_instructor_courses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_my_instructor_courses_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's instructor courses count
  data, status_code, headers = api_instance.get_my_instructor_courses_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_courses_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_instructor_profiles_async

> <InstructorProfileDtoIReadOnlyListEnvelope> get_my_instructor_profiles_async(opts)

Get current user's instructor profiles

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's instructor profiles
  result = api_instance.get_my_instructor_profiles_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_profiles_async: #{e}"
end
```

#### Using the get_my_instructor_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InstructorProfileDtoIReadOnlyListEnvelope>, Integer, Hash)> get_my_instructor_profiles_async_with_http_info(opts)

```ruby
begin
  # Get current user's instructor profiles
  data, status_code, headers = api_instance.get_my_instructor_profiles_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InstructorProfileDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**InstructorProfileDtoIReadOnlyListEnvelope**](InstructorProfileDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_instructor_profiles_count_async

> Integer get_my_instructor_profiles_count_async(opts)

Get current user's instructor profiles count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's instructor profiles count
  result = api_instance.get_my_instructor_profiles_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_profiles_count_async: #{e}"
end
```

#### Using the get_my_instructor_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_my_instructor_profiles_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's instructor profiles count
  data, status_code, headers = api_instance.get_my_instructor_profiles_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_instructor_profiles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_pending_task_count_async

> <CountDtoEnvelope> get_my_pending_task_count_async(opts)

Get current user's pending task count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's pending task count
  result = api_instance.get_my_pending_task_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_pending_task_count_async: #{e}"
end
```

#### Using the get_my_pending_task_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CountDtoEnvelope>, Integer, Hash)> get_my_pending_task_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's pending task count
  data, status_code, headers = api_instance.get_my_pending_task_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CountDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_pending_task_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CountDtoEnvelope**](CountDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_student_courses_async

> <CourseDtoIReadOnlyListEnvelope> get_my_student_courses_async(opts)

Get current user's enrolled courses

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's enrolled courses
  result = api_instance.get_my_student_courses_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_courses_async: #{e}"
end
```

#### Using the get_my_student_courses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseDtoIReadOnlyListEnvelope>, Integer, Hash)> get_my_student_courses_async_with_http_info(opts)

```ruby
begin
  # Get current user's enrolled courses
  data, status_code, headers = api_instance.get_my_student_courses_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_courses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseDtoIReadOnlyListEnvelope**](CourseDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_student_courses_count_async

> Integer get_my_student_courses_count_async(opts)

Get current user's enrolled courses count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's enrolled courses count
  result = api_instance.get_my_student_courses_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_courses_count_async: #{e}"
end
```

#### Using the get_my_student_courses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_my_student_courses_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's enrolled courses count
  data, status_code, headers = api_instance.get_my_student_courses_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_courses_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_student_profiles_async

> <StudentProfileDtoIReadOnlyListEnvelope> get_my_student_profiles_async(opts)

Get current user's student profiles

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's student profiles
  result = api_instance.get_my_student_profiles_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_profiles_async: #{e}"
end
```

#### Using the get_my_student_profiles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StudentProfileDtoIReadOnlyListEnvelope>, Integer, Hash)> get_my_student_profiles_async_with_http_info(opts)

```ruby
begin
  # Get current user's student profiles
  data, status_code, headers = api_instance.get_my_student_profiles_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StudentProfileDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_profiles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**StudentProfileDtoIReadOnlyListEnvelope**](StudentProfileDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_my_student_profiles_count_async

> Integer get_my_student_profiles_count_async(opts)

Get current user's student profiles count

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MeApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get current user's student profiles count
  result = api_instance.get_my_student_profiles_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_profiles_count_async: #{e}"
end
```

#### Using the get_my_student_profiles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_my_student_profiles_count_async_with_http_info(opts)

```ruby
begin
  # Get current user's student profiles count
  data, status_code, headers = api_instance.get_my_student_profiles_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling MeApi->get_my_student_profiles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

