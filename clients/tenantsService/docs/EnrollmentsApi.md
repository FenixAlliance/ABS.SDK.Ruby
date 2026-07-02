# OpenapiClient::EnrollmentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_enrollment**](EnrollmentsApi.md#create_tenant_enrollment) | **POST** /api/v2/TenantsService/Enrollments | Create a new tenant enrollment |
| [**delete_tenant_enrollment**](EnrollmentsApi.md#delete_tenant_enrollment) | **DELETE** /api/v2/TenantsService/Enrollments/{enrollmentId} | Delete a tenant enrollment |
| [**get_extended_tenant_enrollments**](EnrollmentsApi.md#get_extended_tenant_enrollments) | **GET** /api/v2/TenantsService/Enrollments/Extended | Retrieve a list of tenant enrollments |
| [**get_extended_tenant_enrollments_count**](EnrollmentsApi.md#get_extended_tenant_enrollments_count) | **GET** /api/v2/TenantsService/Enrollments/Extended/Count | Get the count of tenant enrollments |
| [**get_tenant_enrollment_by_id**](EnrollmentsApi.md#get_tenant_enrollment_by_id) | **GET** /api/v2/TenantsService/Enrollments/{enrollmentId} | Retrieve a single tenant enrollment by its ID |
| [**get_tenant_enrollments**](EnrollmentsApi.md#get_tenant_enrollments) | **GET** /api/v2/TenantsService/Enrollments | Retrieve a list of tenant enrollments |
| [**get_tenant_enrollments_count**](EnrollmentsApi.md#get_tenant_enrollments_count) | **GET** /api/v2/TenantsService/Enrollments/Count | Get the count of tenant enrollments |
| [**patch_tenant_enrollment_async**](EnrollmentsApi.md#patch_tenant_enrollment_async) | **PATCH** /api/v2/TenantsService/Enrollments/{enrollmentId} | Patch a tenant enrollment |
| [**update_tenant_enrollment**](EnrollmentsApi.md#update_tenant_enrollment) | **PUT** /api/v2/TenantsService/Enrollments/{enrollmentId} | Update a tenant enrollment |


## create_tenant_enrollment

> <EmptyEnvelope> create_tenant_enrollment(tenant_id, opts)

Create a new tenant enrollment

Create a new tenant enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_enrollment_create_dto: OpenapiClient::TenantEnrollmentCreateDto.new # TenantEnrollmentCreateDto | 
}

begin
  # Create a new tenant enrollment
  result = api_instance.create_tenant_enrollment(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->create_tenant_enrollment: #{e}"
end
```

#### Using the create_tenant_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_enrollment_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant enrollment
  data, status_code, headers = api_instance.create_tenant_enrollment_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->create_tenant_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_enrollment_create_dto** | [**TenantEnrollmentCreateDto**](TenantEnrollmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_enrollment

> <EmptyEnvelope> delete_tenant_enrollment(tenant_id, enrollment_id, opts)

Delete a tenant enrollment

Delete a tenant enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant enrollment
  result = api_instance.delete_tenant_enrollment(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->delete_tenant_enrollment: #{e}"
end
```

#### Using the delete_tenant_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_enrollment_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Delete a tenant enrollment
  data, status_code, headers = api_instance.delete_tenant_enrollment_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->delete_tenant_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_tenant_enrollments

> <TenantEnrollmentDtoListEnvelope> get_extended_tenant_enrollments(tenant_id, opts)

Retrieve a list of tenant enrollments

Retrieve a list of tenant enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant enrollments
  result = api_instance.get_extended_tenant_enrollments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_extended_tenant_enrollments: #{e}"
end
```

#### Using the get_extended_tenant_enrollments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_extended_tenant_enrollments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant enrollments
  data, status_code, headers = api_instance.get_extended_tenant_enrollments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_extended_tenant_enrollments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_tenant_enrollments_count

> <Int32Envelope> get_extended_tenant_enrollments_count(tenant_id, opts)

Get the count of tenant enrollments

Get the count of tenant enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant enrollments
  result = api_instance.get_extended_tenant_enrollments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_extended_tenant_enrollments_count: #{e}"
end
```

#### Using the get_extended_tenant_enrollments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_extended_tenant_enrollments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant enrollments
  data, status_code, headers = api_instance.get_extended_tenant_enrollments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_extended_tenant_enrollments_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_enrollment_by_id

> <TenantEnrollmentDtoEnvelope> get_tenant_enrollment_by_id(tenant_id, enrollment_id, user_id, opts)

Retrieve a single tenant enrollment by its ID

Retrieve a single tenant enrollment by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant enrollment by its ID
  result = api_instance.get_tenant_enrollment_by_id(tenant_id, enrollment_id, user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_tenant_enrollment_by_id: #{e}"
end
```

#### Using the get_tenant_enrollment_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoEnvelope>, Integer, Hash)> get_tenant_enrollment_by_id_with_http_info(tenant_id, enrollment_id, user_id, opts)

```ruby
begin
  # Retrieve a single tenant enrollment by its ID
  data, status_code, headers = api_instance.get_tenant_enrollment_by_id_with_http_info(tenant_id, enrollment_id, user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_tenant_enrollment_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoEnvelope**](TenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_enrollments

> <TenantEnrollmentDtoListEnvelope> get_tenant_enrollments(tenant_id, opts)

Retrieve a list of tenant enrollments

Retrieve a list of tenant enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant enrollments
  result = api_instance.get_tenant_enrollments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_tenant_enrollments: #{e}"
end
```

#### Using the get_tenant_enrollments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_tenant_enrollments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant enrollments
  data, status_code, headers = api_instance.get_tenant_enrollments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_tenant_enrollments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_enrollments_count

> <Int32Envelope> get_tenant_enrollments_count(tenant_id, opts)

Get the count of tenant enrollments

Get the count of tenant enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant enrollments
  result = api_instance.get_tenant_enrollments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_tenant_enrollments_count: #{e}"
end
```

#### Using the get_tenant_enrollments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_enrollments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant enrollments
  data, status_code, headers = api_instance.get_tenant_enrollments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->get_tenant_enrollments_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_tenant_enrollment_async

> <EmptyEnvelope> patch_tenant_enrollment_async(tenant_id, enrollment_id, opts)

Patch a tenant enrollment

Patch a tenant enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a tenant enrollment
  result = api_instance.patch_tenant_enrollment_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->patch_tenant_enrollment_async: #{e}"
end
```

#### Using the patch_tenant_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tenant_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Patch a tenant enrollment
  data, status_code, headers = api_instance.patch_tenant_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->patch_tenant_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
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


## update_tenant_enrollment

> <EmptyEnvelope> update_tenant_enrollment(tenant_id, enrollment_id, opts)

Update a tenant enrollment

Update a tenant enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_enrollment_update_dto: OpenapiClient::TenantEnrollmentUpdateDto.new # TenantEnrollmentUpdateDto | 
}

begin
  # Update a tenant enrollment
  result = api_instance.update_tenant_enrollment(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->update_tenant_enrollment: #{e}"
end
```

#### Using the update_tenant_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_enrollment_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Update a tenant enrollment
  data, status_code, headers = api_instance.update_tenant_enrollment_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EnrollmentsApi->update_tenant_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_enrollment_update_dto** | [**TenantEnrollmentUpdateDto**](TenantEnrollmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

