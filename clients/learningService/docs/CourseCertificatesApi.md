# OpenapiClient::CourseCertificatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_course_certificate_async**](CourseCertificatesApi.md#create_course_certificate_async) | **POST** /api/v2/LearningService/CourseCertificates | Create a course certificate |
| [**create_course_certificate_template_async**](CourseCertificatesApi.md#create_course_certificate_template_async) | **POST** /api/v2/LearningService/CourseCertificates/Template | Create a certificate template |
| [**delete_course_certificate_async**](CourseCertificatesApi.md#delete_course_certificate_async) | **DELETE** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Delete a course certificate |
| [**delete_course_certificate_template_async**](CourseCertificatesApi.md#delete_course_certificate_template_async) | **DELETE** /api/v2/LearningService/CourseCertificates/Template/{courseCertificateTemplateId} | Delete a certificate template |
| [**get_course_certificate_async**](CourseCertificatesApi.md#get_course_certificate_async) | **GET** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Get course certificate by ID |
| [**get_course_certificate_template_async**](CourseCertificatesApi.md#get_course_certificate_template_async) | **GET** /api/v2/LearningService/CourseCertificates/Template/{courseCertificateTemplateId} | Get certificate template by ID |
| [**get_course_certificate_templates_async**](CourseCertificatesApi.md#get_course_certificate_templates_async) | **GET** /api/v2/LearningService/CourseCertificates/Template | Get all certificate templates |
| [**get_course_certificate_templates_count_async**](CourseCertificatesApi.md#get_course_certificate_templates_count_async) | **GET** /api/v2/LearningService/CourseCertificates/Template/Count | Get certificate templates count |
| [**get_course_certificates_async**](CourseCertificatesApi.md#get_course_certificates_async) | **GET** /api/v2/LearningService/CourseCertificates | Get all course certificates |
| [**get_course_certificates_count_async**](CourseCertificatesApi.md#get_course_certificates_count_async) | **GET** /api/v2/LearningService/CourseCertificates/Count | Get course certificates count |
| [**patch_course_certificate_async**](CourseCertificatesApi.md#patch_course_certificate_async) | **PATCH** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Patch a course certificate |
| [**patch_course_certificate_template_async**](CourseCertificatesApi.md#patch_course_certificate_template_async) | **PATCH** /api/v2/LearningService/CourseCertificates/Template/{courseCertificateTemplateId} | Patch a certificate template |
| [**update_course_certificate_async**](CourseCertificatesApi.md#update_course_certificate_async) | **PUT** /api/v2/LearningService/CourseCertificates/{courseCertificateId} | Update a course certificate |
| [**update_course_certificate_template_async**](CourseCertificatesApi.md#update_course_certificate_template_async) | **PUT** /api/v2/LearningService/CourseCertificates/Template/{courseCertificateTemplateId} | Update a certificate template |


## create_course_certificate_async

> create_course_certificate_async(tenant_id, opts)

Create a course certificate

Creates a new course certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_completion_certificate_create_dto: OpenapiClient::CourseCompletionCertificateCreateDto.new({student_profile_id: 'student_profile_id_example', course_enrollment_id: 'course_enrollment_id_example'}) # CourseCompletionCertificateCreateDto | 
}

begin
  # Create a course certificate
  api_instance.create_course_certificate_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->create_course_certificate_async: #{e}"
end
```

#### Using the create_course_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_certificate_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a course certificate
  data, status_code, headers = api_instance.create_course_certificate_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->create_course_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_completion_certificate_create_dto** | [**CourseCompletionCertificateCreateDto**](CourseCompletionCertificateCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_course_certificate_template_async

> create_course_certificate_template_async(tenant_id, opts)

Create a certificate template

Creates a new course certificate template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_certificate_template_create_dto: OpenapiClient::CourseCertificateTemplateCreateDto.new({course_id: 'course_id_example'}) # CourseCertificateTemplateCreateDto | 
}

begin
  # Create a certificate template
  api_instance.create_course_certificate_template_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->create_course_certificate_template_async: #{e}"
end
```

#### Using the create_course_certificate_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_course_certificate_template_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a certificate template
  data, status_code, headers = api_instance.create_course_certificate_template_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->create_course_certificate_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_certificate_template_create_dto** | [**CourseCertificateTemplateCreateDto**](CourseCertificateTemplateCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_course_certificate_async

> delete_course_certificate_async(tenant_id, course_certificate_id, opts)

Delete a course certificate

Deletes a course certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a course certificate
  api_instance.delete_course_certificate_async(tenant_id, course_certificate_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->delete_course_certificate_async: #{e}"
end
```

#### Using the delete_course_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)

```ruby
begin
  # Delete a course certificate
  data, status_code, headers = api_instance.delete_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->delete_course_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_course_certificate_template_async

> delete_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)

Delete a certificate template

Deletes a course certificate template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a certificate template
  api_instance.delete_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->delete_course_certificate_template_async: #{e}"
end
```

#### Using the delete_course_certificate_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)

```ruby
begin
  # Delete a certificate template
  data, status_code, headers = api_instance.delete_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->delete_course_certificate_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_certificate_async

> <CourseCompletionCertificateDto> get_course_certificate_async(tenant_id, course_certificate_id, opts)

Get course certificate by ID

Retrieves a specific course certificate by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course certificate by ID
  result = api_instance.get_course_certificate_async(tenant_id, course_certificate_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_async: #{e}"
end
```

#### Using the get_course_certificate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseCompletionCertificateDto>, Integer, Hash)> get_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)

```ruby
begin
  # Get course certificate by ID
  data, status_code, headers = api_instance.get_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseCompletionCertificateDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseCompletionCertificateDto**](CourseCompletionCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_certificate_template_async

> <CourseCertificateTemplateDto> get_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)

Get certificate template by ID

Retrieves a specific course certificate template by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get certificate template by ID
  result = api_instance.get_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_template_async: #{e}"
end
```

#### Using the get_course_certificate_template_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CourseCertificateTemplateDto>, Integer, Hash)> get_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)

```ruby
begin
  # Get certificate template by ID
  data, status_code, headers = api_instance.get_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CourseCertificateTemplateDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CourseCertificateTemplateDto**](CourseCertificateTemplateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_certificate_templates_async

> <Array<CourseCertificateTemplateDto>> get_course_certificate_templates_async(tenant_id, opts)

Get all certificate templates

Retrieves all course certificate templates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all certificate templates
  result = api_instance.get_course_certificate_templates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_templates_async: #{e}"
end
```

#### Using the get_course_certificate_templates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseCertificateTemplateDto>>, Integer, Hash)> get_course_certificate_templates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all certificate templates
  data, status_code, headers = api_instance.get_course_certificate_templates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseCertificateTemplateDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_templates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseCertificateTemplateDto&gt;**](CourseCertificateTemplateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_certificate_templates_count_async

> Integer get_course_certificate_templates_count_async(tenant_id, opts)

Get certificate templates count

Returns the count of course certificate templates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get certificate templates count
  result = api_instance.get_course_certificate_templates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_templates_count_async: #{e}"
end
```

#### Using the get_course_certificate_templates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_certificate_templates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get certificate templates count
  data, status_code, headers = api_instance.get_course_certificate_templates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificate_templates_count_async_with_http_info: #{e}"
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


## get_course_certificates_async

> <Array<CourseCompletionCertificateDto>> get_course_certificates_async(tenant_id, opts)

Get all course certificates

Retrieves all course certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all course certificates
  result = api_instance.get_course_certificates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificates_async: #{e}"
end
```

#### Using the get_course_certificates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CourseCompletionCertificateDto>>, Integer, Hash)> get_course_certificates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all course certificates
  data, status_code, headers = api_instance.get_course_certificates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CourseCompletionCertificateDto>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Array&lt;CourseCompletionCertificateDto&gt;**](CourseCompletionCertificateDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_course_certificates_count_async

> Integer get_course_certificates_count_async(tenant_id, opts)

Get course certificates count

Returns the count of course certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get course certificates count
  result = api_instance.get_course_certificates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificates_count_async: #{e}"
end
```

#### Using the get_course_certificates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Integer, Integer, Hash)> get_course_certificates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get course certificates count
  data, status_code, headers = api_instance.get_course_certificates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Integer
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->get_course_certificates_count_async_with_http_info: #{e}"
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


## patch_course_certificate_async

> <EmptyEnvelope> patch_course_certificate_async(tenant_id, course_certificate_id, opts)

Patch a course certificate

Partially updates a course certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a course certificate
  result = api_instance.patch_course_certificate_async(tenant_id, course_certificate_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->patch_course_certificate_async: #{e}"
end
```

#### Using the patch_course_certificate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)

```ruby
begin
  # Patch a course certificate
  data, status_code, headers = api_instance.patch_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->patch_course_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_id** | **String** |  |  |
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


## patch_course_certificate_template_async

> <EmptyEnvelope> patch_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)

Patch a certificate template

Partially updates a course certificate template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a certificate template
  result = api_instance.patch_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->patch_course_certificate_template_async: #{e}"
end
```

#### Using the patch_course_certificate_template_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)

```ruby
begin
  # Patch a certificate template
  data, status_code, headers = api_instance.patch_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->patch_course_certificate_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_template_id** | **String** |  |  |
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


## update_course_certificate_async

> update_course_certificate_async(tenant_id, course_certificate_id, opts)

Update a course certificate

Updates an existing course certificate for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_completion_certificate_update_dto: OpenapiClient::CourseCompletionCertificateUpdateDto.new # CourseCompletionCertificateUpdateDto | 
}

begin
  # Update a course certificate
  api_instance.update_course_certificate_async(tenant_id, course_certificate_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->update_course_certificate_async: #{e}"
end
```

#### Using the update_course_certificate_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)

```ruby
begin
  # Update a course certificate
  data, status_code, headers = api_instance.update_course_certificate_async_with_http_info(tenant_id, course_certificate_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->update_course_certificate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_completion_certificate_update_dto** | [**CourseCompletionCertificateUpdateDto**](CourseCompletionCertificateUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_course_certificate_template_async

> update_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)

Update a certificate template

Updates an existing course certificate template for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CourseCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
course_certificate_template_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  course_certificate_template_update_dto: OpenapiClient::CourseCertificateTemplateUpdateDto.new # CourseCertificateTemplateUpdateDto | 
}

begin
  # Update a certificate template
  api_instance.update_course_certificate_template_async(tenant_id, course_certificate_template_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->update_course_certificate_template_async: #{e}"
end
```

#### Using the update_course_certificate_template_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)

```ruby
begin
  # Update a certificate template
  data, status_code, headers = api_instance.update_course_certificate_template_async_with_http_info(tenant_id, course_certificate_template_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CourseCertificatesApi->update_course_certificate_template_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **course_certificate_template_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **course_certificate_template_update_dto** | [**CourseCertificateTemplateUpdateDto**](CourseCertificateTemplateUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

