# OpenapiClient::CoursesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_async**](CoursesApi.md#create_course_async) | **POST** /api/v2/LearningService/Courses | Create a new course |
| [**delete_course_async**](CoursesApi.md#delete_course_async) | **DELETE** /api/v2/LearningService/Courses/{courseId} | Delete a course |
| [**get_course_articles_by_course_wiki_async**](CoursesApi.md#get_course_articles_by_course_wiki_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Articles/{wikiId} | Get course articles by course wiki |
| [**get_course_articles_by_course_wiki_count_async**](CoursesApi.md#get_course_articles_by_course_wiki_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Articles/{wikiId}/Count | Get course articles by course wiki count |
| [**get_course_assignments_by_course_async**](CoursesApi.md#get_course_assignments_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Assignments | Get course assignments by course |
| [**get_course_assignments_by_course_count_async**](CoursesApi.md#get_course_assignments_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Assignments/Count | Get course assignments by course count |
| [**get_course_by_id_async**](CoursesApi.md#get_course_by_id_async) | **GET** /api/v2/LearningService/Courses/{courseId} | Get course by ID |
| [**get_course_categories_by_course_async**](CoursesApi.md#get_course_categories_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Categories | Get course categories by course |
| [**get_course_categories_by_course_count_async**](CoursesApi.md#get_course_categories_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Categories/Count | Get course categories by course count |
| [**get_course_cohorts_by_course_async**](CoursesApi.md#get_course_cohorts_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Cohorts | Get course cohorts by course |
| [**get_course_cohorts_by_course_count_async**](CoursesApi.md#get_course_cohorts_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Cohorts/Count | Get course cohorts by course count |
| [**get_course_enrollments_by_course_async**](CoursesApi.md#get_course_enrollments_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Enrollments | Get enrollments by course |
| [**get_course_files_by_course_async**](CoursesApi.md#get_course_files_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Files | Get course files by course |
| [**get_course_files_by_course_count_async**](CoursesApi.md#get_course_files_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Files/Count | Get course files by course count |
| [**get_course_forums_by_course_async**](CoursesApi.md#get_course_forums_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Forums | Get course forums by course |
| [**get_course_forums_by_course_count_async**](CoursesApi.md#get_course_forums_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Forums/Count | Get course forums by course count |
| [**get_course_handouts_by_course_async**](CoursesApi.md#get_course_handouts_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Handouts | Get course handouts by course |
| [**get_course_handouts_by_course_count_async**](CoursesApi.md#get_course_handouts_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Handouts/Count | Get course handouts by course count |
| [**get_course_libraries_by_course_async**](CoursesApi.md#get_course_libraries_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Libraries | Get course libraries by course |
| [**get_course_libraries_by_course_count_async**](CoursesApi.md#get_course_libraries_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Libraries/Count | Get course libraries by course count |
| [**get_course_pages_by_course_async**](CoursesApi.md#get_course_pages_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Pages | Get course pages by course |
| [**get_course_pages_by_course_count_async**](CoursesApi.md#get_course_pages_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Pages/Count | Get course pages by course count |
| [**get_course_problem_sets_by_course_async**](CoursesApi.md#get_course_problem_sets_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ProblemSets | Get course problem sets by course |
| [**get_course_problem_sets_by_course_count_async**](CoursesApi.md#get_course_problem_sets_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/ProblemSets/Count | Get course problem sets by course count |
| [**get_course_sections_by_course_async**](CoursesApi.md#get_course_sections_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Sections | Get course sections by course |
| [**get_course_sections_by_course_count_async**](CoursesApi.md#get_course_sections_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Sections/Count | Get course sections by course count |
| [**get_course_unit_components_by_course_async**](CoursesApi.md#get_course_unit_components_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/UnitComponents | Get course unit components by course |
| [**get_course_unit_components_by_course_count_async**](CoursesApi.md#get_course_unit_components_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/UnitComponents/Count | Get course unit components by course count |
| [**get_course_units_by_section_async**](CoursesApi.md#get_course_units_by_section_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Units/{sectionId} | Get course units by section |
| [**get_course_units_by_section_count_async**](CoursesApi.md#get_course_units_by_section_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Units/{sectionId}/Count | Get course units by section count |
| [**get_course_updates_by_course_async**](CoursesApi.md#get_course_updates_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Updates | Get course updates by course |
| [**get_course_updates_by_course_count_async**](CoursesApi.md#get_course_updates_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Updates/Count | Get course updates by course count |
| [**get_course_wikis_by_course_async**](CoursesApi.md#get_course_wikis_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Wikis | Get course wikis by course |
| [**get_course_wikis_by_course_count_async**](CoursesApi.md#get_course_wikis_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Wikis/Count | Get course wikis by course count |
| [**get_courses_async**](CoursesApi.md#get_courses_async) | **GET** /api/v2/LearningService/Courses | Get courses |
| [**get_courses_count_async**](CoursesApi.md#get_courses_count_async) | **GET** /api/v2/LearningService/Courses/Count | Get courses count |
| [**get_instructor_profiles_by_course_async**](CoursesApi.md#get_instructor_profiles_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Instructors | Get instructor profiles by course |
| [**get_instructor_profiles_by_course_count_async**](CoursesApi.md#get_instructor_profiles_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Instructors/Count | Get instructor profiles by course count |
| [**get_student_profiles_by_course_async**](CoursesApi.md#get_student_profiles_by_course_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Students | Get student profiles by course |
| [**get_student_profiles_by_course_count_async**](CoursesApi.md#get_student_profiles_by_course_count_async) | **GET** /api/v2/LearningService/Courses/{courseId}/Students/Count | Get student profiles by course count |
| [**update_course_async**](CoursesApi.md#update_course_async) | **PUT** /api/v2/LearningService/Courses/{courseId} | Update a course |


## create_course_async

> create_course_async(tenant_id, opts)

Create a new course

Creates a new course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_create_dto: OpenapiClient::CourseCreateDto.new # CourseCreateDto | 
}

begin
  # Create a new course
  api_instance.create_course_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->create_course_async: #{e}"
end
```

#### Using the create_course_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new course
  data, status_code, headers = api_instance.create_course_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->create_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_create_dto** | [**CourseCreateDto**](CourseCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_async

> delete_course_async(tenant_id, course_id, opts)

Delete a course

Deletes a course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course
  api_instance.delete_course_async(tenant_id, course_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->delete_course_async: #{e}"
end
```

#### Using the delete_course_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Delete a course
  data, status_code, headers = api_instance.delete_course_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->delete_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_articles_by_course_wiki_async

> <Array<CourseArticleDto>> get_course_articles_by_course_wiki_async(course_id, wiki_id, opts)

Get course articles by course wiki

Retrieves all course articles for a specific course wiki.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
wiki_id = 'wiki_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course articles by course wiki
  result = api_instance.get_course_articles_by_course_wiki_async(course_id, wiki_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_articles_by_course_wiki_async: #{e}"
end
```

#### Using the get_course_articles_by_course_wiki_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseArticleDto>>, Integer, Hash)> get_course_articles_by_course_wiki_async_with_http_info(course_id, wiki_id, opts)

```ruby
begin
  # Get course articles by course wiki
  data, status_code, headers = api_instance.get_course_articles_by_course_wiki_async_with_http_info(course_id, wiki_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseArticleDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_articles_by_course_wiki_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **wiki_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseArticleDto&gt;**](CourseArticleDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_articles_by_course_wiki_count_async

> Integer get_course_articles_by_course_wiki_count_async(course_id, wiki_id, opts)

Get course articles by course wiki count

Returns the count of course articles for a specific course wiki.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
wiki_id = 'wiki_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course articles by course wiki count
  result = api_instance.get_course_articles_by_course_wiki_count_async(course_id, wiki_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_articles_by_course_wiki_count_async: #{e}"
end
```

#### Using the get_course_articles_by_course_wiki_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_articles_by_course_wiki_count_async_with_http_info(course_id, wiki_id, opts)

```ruby
begin
  # Get course articles by course wiki count
  data, status_code, headers = api_instance.get_course_articles_by_course_wiki_count_async_with_http_info(course_id, wiki_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_articles_by_course_wiki_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **wiki_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignments_by_course_async

> <Array<CourseAssignmentDto>> get_course_assignments_by_course_async(course_id, opts)

Get course assignments by course

Retrieves all course assignments for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course assignments by course
  result = api_instance.get_course_assignments_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_assignments_by_course_async: #{e}"
end
```

#### Using the get_course_assignments_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseAssignmentDto>>, Integer, Hash)> get_course_assignments_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course assignments by course
  data, status_code, headers = api_instance.get_course_assignments_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseAssignmentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_assignments_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseAssignmentDto&gt;**](CourseAssignmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_assignments_by_course_count_async

> Integer get_course_assignments_by_course_count_async(course_id, opts)

Get course assignments by course count

Returns the count of course assignments for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course assignments by course count
  result = api_instance.get_course_assignments_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_assignments_by_course_count_async: #{e}"
end
```

#### Using the get_course_assignments_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_assignments_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course assignments by course count
  data, status_code, headers = api_instance.get_course_assignments_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_assignments_by_course_count_async_with_http_info: #{e}"
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


## get_course_by_id_async

> <CourseDto> get_course_by_id_async(tenant_id, course_id, opts)

Get course by ID

Retrieves a specific course by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course by ID
  result = api_instance.get_course_by_id_async(tenant_id, course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_by_id_async: #{e}"
end
```

#### Using the get_course_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseDto>, Integer, Hash)> get_course_by_id_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Get course by ID
  data, status_code, headers = api_instance.get_course_by_id_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseDto**](CourseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_categories_by_course_async

> <Array<CourseCategoryDto>> get_course_categories_by_course_async(course_id, opts)

Get course categories by course

Retrieves all course categories for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course categories by course
  result = api_instance.get_course_categories_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_categories_by_course_async: #{e}"
end
```

#### Using the get_course_categories_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseCategoryDto>>, Integer, Hash)> get_course_categories_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course categories by course
  data, status_code, headers = api_instance.get_course_categories_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseCategoryDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_categories_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseCategoryDto&gt;**](CourseCategoryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_categories_by_course_count_async

> Integer get_course_categories_by_course_count_async(course_id, opts)

Get course categories by course count

Returns the count of course categories for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course categories by course count
  result = api_instance.get_course_categories_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_categories_by_course_count_async: #{e}"
end
```

#### Using the get_course_categories_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_categories_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course categories by course count
  data, status_code, headers = api_instance.get_course_categories_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_categories_by_course_count_async_with_http_info: #{e}"
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


## get_course_cohorts_by_course_async

> <Array<CourseCohortDto>> get_course_cohorts_by_course_async(course_id, opts)

Get course cohorts by course

Retrieves all course cohorts for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course cohorts by course
  result = api_instance.get_course_cohorts_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_cohorts_by_course_async: #{e}"
end
```

#### Using the get_course_cohorts_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseCohortDto>>, Integer, Hash)> get_course_cohorts_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course cohorts by course
  data, status_code, headers = api_instance.get_course_cohorts_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseCohortDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_cohorts_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseCohortDto&gt;**](CourseCohortDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_cohorts_by_course_count_async

> Integer get_course_cohorts_by_course_count_async(course_id, opts)

Get course cohorts by course count

Returns the count of course cohorts for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course cohorts by course count
  result = api_instance.get_course_cohorts_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_cohorts_by_course_count_async: #{e}"
end
```

#### Using the get_course_cohorts_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_cohorts_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course cohorts by course count
  data, status_code, headers = api_instance.get_course_cohorts_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_cohorts_by_course_count_async_with_http_info: #{e}"
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


## get_course_enrollments_by_course_async

> <Array<CourseEnrollmentDto>> get_course_enrollments_by_course_async(tenant_id, course_id, opts)

Get enrollments by course

Retrieves all enrollments for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get enrollments by course
  result = api_instance.get_course_enrollments_by_course_async(tenant_id, course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_enrollments_by_course_async: #{e}"
end
```

#### Using the get_course_enrollments_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseEnrollmentDto>>, Integer, Hash)> get_course_enrollments_by_course_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Get enrollments by course
  data, status_code, headers = api_instance.get_course_enrollments_by_course_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseEnrollmentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_enrollments_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseEnrollmentDto&gt;**](CourseEnrollmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_files_by_course_async

> <Array<CourseFileDto>> get_course_files_by_course_async(course_id, opts)

Get course files by course

Retrieves all course files for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course files by course
  result = api_instance.get_course_files_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_files_by_course_async: #{e}"
end
```

#### Using the get_course_files_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseFileDto>>, Integer, Hash)> get_course_files_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course files by course
  data, status_code, headers = api_instance.get_course_files_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseFileDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_files_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseFileDto&gt;**](CourseFileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_files_by_course_count_async

> Integer get_course_files_by_course_count_async(course_id, opts)

Get course files by course count

Returns the count of course files for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course files by course count
  result = api_instance.get_course_files_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_files_by_course_count_async: #{e}"
end
```

#### Using the get_course_files_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_files_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course files by course count
  data, status_code, headers = api_instance.get_course_files_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_files_by_course_count_async_with_http_info: #{e}"
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


## get_course_forums_by_course_async

> <Array<CourseForumDto>> get_course_forums_by_course_async(course_id, opts)

Get course forums by course

Retrieves all course forums for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course forums by course
  result = api_instance.get_course_forums_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_forums_by_course_async: #{e}"
end
```

#### Using the get_course_forums_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseForumDto>>, Integer, Hash)> get_course_forums_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course forums by course
  data, status_code, headers = api_instance.get_course_forums_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseForumDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_forums_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseForumDto&gt;**](CourseForumDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_forums_by_course_count_async

> Integer get_course_forums_by_course_count_async(course_id, opts)

Get course forums by course count

Returns the count of course forums for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course forums by course count
  result = api_instance.get_course_forums_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_forums_by_course_count_async: #{e}"
end
```

#### Using the get_course_forums_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_forums_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course forums by course count
  data, status_code, headers = api_instance.get_course_forums_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_forums_by_course_count_async_with_http_info: #{e}"
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


## get_course_handouts_by_course_async

> <Array<CourseHandoutDto>> get_course_handouts_by_course_async(course_id, opts)

Get course handouts by course

Retrieves all course handouts for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course handouts by course
  result = api_instance.get_course_handouts_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_handouts_by_course_async: #{e}"
end
```

#### Using the get_course_handouts_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseHandoutDto>>, Integer, Hash)> get_course_handouts_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course handouts by course
  data, status_code, headers = api_instance.get_course_handouts_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseHandoutDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_handouts_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseHandoutDto&gt;**](CourseHandoutDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_handouts_by_course_count_async

> Integer get_course_handouts_by_course_count_async(course_id, opts)

Get course handouts by course count

Returns the count of course handouts for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course handouts by course count
  result = api_instance.get_course_handouts_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_handouts_by_course_count_async: #{e}"
end
```

#### Using the get_course_handouts_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_handouts_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course handouts by course count
  data, status_code, headers = api_instance.get_course_handouts_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_handouts_by_course_count_async_with_http_info: #{e}"
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


## get_course_libraries_by_course_async

> <Array<CourseLibraryDto>> get_course_libraries_by_course_async(course_id, opts)

Get course libraries by course

Retrieves all course libraries for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course libraries by course
  result = api_instance.get_course_libraries_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_libraries_by_course_async: #{e}"
end
```

#### Using the get_course_libraries_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseLibraryDto>>, Integer, Hash)> get_course_libraries_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course libraries by course
  data, status_code, headers = api_instance.get_course_libraries_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseLibraryDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_libraries_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseLibraryDto&gt;**](CourseLibraryDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_libraries_by_course_count_async

> Integer get_course_libraries_by_course_count_async(course_id, opts)

Get course libraries by course count

Returns the count of course libraries for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course libraries by course count
  result = api_instance.get_course_libraries_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_libraries_by_course_count_async: #{e}"
end
```

#### Using the get_course_libraries_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_libraries_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course libraries by course count
  data, status_code, headers = api_instance.get_course_libraries_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_libraries_by_course_count_async_with_http_info: #{e}"
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


## get_course_pages_by_course_async

> <Array<CoursePageDto>> get_course_pages_by_course_async(course_id, opts)

Get course pages by course

Retrieves all course pages for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course pages by course
  result = api_instance.get_course_pages_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_pages_by_course_async: #{e}"
end
```

#### Using the get_course_pages_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CoursePageDto>>, Integer, Hash)> get_course_pages_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course pages by course
  data, status_code, headers = api_instance.get_course_pages_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CoursePageDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_pages_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CoursePageDto&gt;**](CoursePageDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_pages_by_course_count_async

> Integer get_course_pages_by_course_count_async(course_id, opts)

Get course pages by course count

Returns the count of course pages for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course pages by course count
  result = api_instance.get_course_pages_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_pages_by_course_count_async: #{e}"
end
```

#### Using the get_course_pages_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_pages_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course pages by course count
  data, status_code, headers = api_instance.get_course_pages_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_pages_by_course_count_async_with_http_info: #{e}"
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


## get_course_problem_sets_by_course_async

> <Array<CourseProblemSetDto>> get_course_problem_sets_by_course_async(course_id, opts)

Get course problem sets by course

Retrieves all course problem sets for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course problem sets by course
  result = api_instance.get_course_problem_sets_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_problem_sets_by_course_async: #{e}"
end
```

#### Using the get_course_problem_sets_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseProblemSetDto>>, Integer, Hash)> get_course_problem_sets_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course problem sets by course
  data, status_code, headers = api_instance.get_course_problem_sets_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseProblemSetDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_problem_sets_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseProblemSetDto&gt;**](CourseProblemSetDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_problem_sets_by_course_count_async

> Integer get_course_problem_sets_by_course_count_async(course_id, opts)

Get course problem sets by course count

Returns the count of course problem sets for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course problem sets by course count
  result = api_instance.get_course_problem_sets_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_problem_sets_by_course_count_async: #{e}"
end
```

#### Using the get_course_problem_sets_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_problem_sets_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course problem sets by course count
  data, status_code, headers = api_instance.get_course_problem_sets_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_problem_sets_by_course_count_async_with_http_info: #{e}"
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


## get_course_sections_by_course_async

> <Array<CourseSectionDto>> get_course_sections_by_course_async(course_id, opts)

Get course sections by course

Retrieves all course sections for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course sections by course
  result = api_instance.get_course_sections_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_sections_by_course_async: #{e}"
end
```

#### Using the get_course_sections_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseSectionDto>>, Integer, Hash)> get_course_sections_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course sections by course
  data, status_code, headers = api_instance.get_course_sections_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseSectionDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_sections_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseSectionDto&gt;**](CourseSectionDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_sections_by_course_count_async

> Integer get_course_sections_by_course_count_async(course_id, opts)

Get course sections by course count

Returns the count of course sections for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course sections by course count
  result = api_instance.get_course_sections_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_sections_by_course_count_async: #{e}"
end
```

#### Using the get_course_sections_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_sections_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course sections by course count
  data, status_code, headers = api_instance.get_course_sections_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_sections_by_course_count_async_with_http_info: #{e}"
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


## get_course_unit_components_by_course_async

> <Array<CourseUnitComponentDto>> get_course_unit_components_by_course_async(course_id, opts)

Get course unit components by course

Retrieves all course unit components for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course unit components by course
  result = api_instance.get_course_unit_components_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_unit_components_by_course_async: #{e}"
end
```

#### Using the get_course_unit_components_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseUnitComponentDto>>, Integer, Hash)> get_course_unit_components_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course unit components by course
  data, status_code, headers = api_instance.get_course_unit_components_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseUnitComponentDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_unit_components_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseUnitComponentDto&gt;**](CourseUnitComponentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_unit_components_by_course_count_async

> Integer get_course_unit_components_by_course_count_async(course_id, opts)

Get course unit components by course count

Returns the count of course unit components for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course unit components by course count
  result = api_instance.get_course_unit_components_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_unit_components_by_course_count_async: #{e}"
end
```

#### Using the get_course_unit_components_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_unit_components_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course unit components by course count
  data, status_code, headers = api_instance.get_course_unit_components_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_unit_components_by_course_count_async_with_http_info: #{e}"
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


## get_course_units_by_section_async

> <Array<CourseUnitDto>> get_course_units_by_section_async(course_id, section_id, opts)

Get course units by section

Retrieves all course units for a specific course section.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
section_id = 'section_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course units by section
  result = api_instance.get_course_units_by_section_async(course_id, section_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_units_by_section_async: #{e}"
end
```

#### Using the get_course_units_by_section_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseUnitDto>>, Integer, Hash)> get_course_units_by_section_async_with_http_info(course_id, section_id, opts)

```ruby
begin
  # Get course units by section
  data, status_code, headers = api_instance.get_course_units_by_section_async_with_http_info(course_id, section_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseUnitDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_units_by_section_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **section_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseUnitDto&gt;**](CourseUnitDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_units_by_section_count_async

> Integer get_course_units_by_section_count_async(course_id, section_id, opts)

Get course units by section count

Returns the count of course units for a specific course section.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
section_id = 'section_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course units by section count
  result = api_instance.get_course_units_by_section_count_async(course_id, section_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_units_by_section_count_async: #{e}"
end
```

#### Using the get_course_units_by_section_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_units_by_section_count_async_with_http_info(course_id, section_id, opts)

```ruby
begin
  # Get course units by section count
  data, status_code, headers = api_instance.get_course_units_by_section_count_async_with_http_info(course_id, section_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_units_by_section_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **section_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Integer**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_updates_by_course_async

> <Array<CourseNewsDto>> get_course_updates_by_course_async(course_id, opts)

Get course updates by course

Retrieves all course updates for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course updates by course
  result = api_instance.get_course_updates_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_updates_by_course_async: #{e}"
end
```

#### Using the get_course_updates_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseNewsDto>>, Integer, Hash)> get_course_updates_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course updates by course
  data, status_code, headers = api_instance.get_course_updates_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseNewsDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_updates_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseNewsDto&gt;**](CourseNewsDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_updates_by_course_count_async

> Integer get_course_updates_by_course_count_async(course_id, opts)

Get course updates by course count

Returns the count of course updates for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course updates by course count
  result = api_instance.get_course_updates_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_updates_by_course_count_async: #{e}"
end
```

#### Using the get_course_updates_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_updates_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course updates by course count
  data, status_code, headers = api_instance.get_course_updates_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_updates_by_course_count_async_with_http_info: #{e}"
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


## get_course_wikis_by_course_async

> <Array<CourseWikiDto>> get_course_wikis_by_course_async(course_id, opts)

Get course wikis by course

Retrieves all course wikis for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course wikis by course
  result = api_instance.get_course_wikis_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_wikis_by_course_async: #{e}"
end
```

#### Using the get_course_wikis_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseWikiDto>>, Integer, Hash)> get_course_wikis_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course wikis by course
  data, status_code, headers = api_instance.get_course_wikis_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseWikiDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_wikis_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseWikiDto&gt;**](CourseWikiDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_wikis_by_course_count_async

> Integer get_course_wikis_by_course_count_async(course_id, opts)

Get course wikis by course count

Returns the count of course wikis for a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course wikis by course count
  result = api_instance.get_course_wikis_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_wikis_by_course_count_async: #{e}"
end
```

#### Using the get_course_wikis_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_wikis_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get course wikis by course count
  data, status_code, headers = api_instance.get_course_wikis_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_course_wikis_by_course_count_async_with_http_info: #{e}"
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


## get_courses_async

> <Array<CourseDto>> get_courses_async(tenant_id, opts)

Get courses

Retrieves courses. When tenantId is provided, returns tenant-scoped courses; otherwise returns all courses.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get courses
  result = api_instance.get_courses_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_courses_async: #{e}"
end
```

#### Using the get_courses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseDto>>, Integer, Hash)> get_courses_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get courses
  data, status_code, headers = api_instance.get_courses_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_courses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseDto&gt;**](CourseDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_courses_count_async

> Integer get_courses_count_async(tenant_id, opts)

Get courses count

Returns the count of courses. When tenantId is provided, returns tenant-scoped count; otherwise returns global count.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get courses count
  result = api_instance.get_courses_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_courses_count_async: #{e}"
end
```

#### Using the get_courses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_courses_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get courses count
  data, status_code, headers = api_instance.get_courses_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_courses_count_async_with_http_info: #{e}"
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


## get_instructor_profiles_by_course_async

> <Array<InstructorProfileDto>> get_instructor_profiles_by_course_async(course_id, opts)

Get instructor profiles by course

Retrieves all instructor profiles teaching a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get instructor profiles by course
  result = api_instance.get_instructor_profiles_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_instructor_profiles_by_course_async: #{e}"
end
```

#### Using the get_instructor_profiles_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<InstructorProfileDto>>, Integer, Hash)> get_instructor_profiles_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get instructor profiles by course
  data, status_code, headers = api_instance.get_instructor_profiles_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<InstructorProfileDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_instructor_profiles_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;InstructorProfileDto&gt;**](InstructorProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_instructor_profiles_by_course_count_async

> Integer get_instructor_profiles_by_course_count_async(course_id, opts)

Get instructor profiles by course count

Returns the count of instructor profiles teaching a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get instructor profiles by course count
  result = api_instance.get_instructor_profiles_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_instructor_profiles_by_course_count_async: #{e}"
end
```

#### Using the get_instructor_profiles_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_instructor_profiles_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get instructor profiles by course count
  data, status_code, headers = api_instance.get_instructor_profiles_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_instructor_profiles_by_course_count_async_with_http_info: #{e}"
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


## get_student_profiles_by_course_async

> <Array<StudentProfileDto>> get_student_profiles_by_course_async(course_id, opts)

Get student profiles by course

Retrieves all student profiles enrolled in a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get student profiles by course
  result = api_instance.get_student_profiles_by_course_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_student_profiles_by_course_async: #{e}"
end
```

#### Using the get_student_profiles_by_course_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<StudentProfileDto>>, Integer, Hash)> get_student_profiles_by_course_async_with_http_info(course_id, opts)

```ruby
begin
  # Get student profiles by course
  data, status_code, headers = api_instance.get_student_profiles_by_course_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<StudentProfileDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_student_profiles_by_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;StudentProfileDto&gt;**](StudentProfileDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_student_profiles_by_course_count_async

> Integer get_student_profiles_by_course_count_async(course_id, opts)

Get student profiles by course count

Returns the count of student profiles enrolled in a specific course.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
course_id = 'course_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get student profiles by course count
  result = api_instance.get_student_profiles_by_course_count_async(course_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_student_profiles_by_course_count_async: #{e}"
end
```

#### Using the get_student_profiles_by_course_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_student_profiles_by_course_count_async_with_http_info(course_id, opts)

```ruby
begin
  # Get student profiles by course count
  data, status_code, headers = api_instance.get_student_profiles_by_course_count_async_with_http_info(course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->get_student_profiles_by_course_count_async_with_http_info: #{e}"
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


## update_course_async

> update_course_async(tenant_id, course_id, opts)

Update a course

Updates an existing course for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CoursesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_update_dto: OpenapiClient::CourseUpdateDto.new # CourseUpdateDto | 
}

begin
  # Update a course
  api_instance.update_course_async(tenant_id, course_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->update_course_async: #{e}"
end
```

#### Using the update_course_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_async_with_http_info(tenant_id, course_id, opts)

```ruby
begin
  # Update a course
  data, status_code, headers = api_instance.update_course_async_with_http_info(tenant_id, course_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CoursesApi->update_course_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_update_dto** | [**CourseUpdateDto**](CourseUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

