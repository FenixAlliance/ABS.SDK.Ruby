# OpenapiClient::EmployeeEnrollmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_employee_enrollment**](EmployeeEnrollmentsApi.md#create_tenant_employee_enrollment) | **POST** /api/v2/TenantsService/EmployeeEnrollments | Create a new tenant employee enrollment |
| [**delete_tenant_employee_enrollment**](EmployeeEnrollmentsApi.md#delete_tenant_employee_enrollment) | **DELETE** /api/v2/TenantsService/EmployeeEnrollments/{tenantEmployeeEnrollmentId} | Delete a tenant employee enrollment |
| [**get_tenant_employee_enrollment_by_id**](EmployeeEnrollmentsApi.md#get_tenant_employee_enrollment_by_id) | **GET** /api/v2/TenantsService/EmployeeEnrollments/{tenantEmployeeEnrollmentId} | Retrieve a single tenant employee enrollment by its ID |
| [**get_tenant_employee_enrollments**](EmployeeEnrollmentsApi.md#get_tenant_employee_enrollments) | **GET** /api/v2/TenantsService/EmployeeEnrollments | Retrieve a list of tenant employee enrollments |
| [**get_tenant_employee_enrollments_count**](EmployeeEnrollmentsApi.md#get_tenant_employee_enrollments_count) | **GET** /api/v2/TenantsService/EmployeeEnrollments/Count | Get the count of tenant employee enrollments |
| [**update_tenant_employee_enrollment**](EmployeeEnrollmentsApi.md#update_tenant_employee_enrollment) | **PUT** /api/v2/TenantsService/EmployeeEnrollments/{tenantEmployeeEnrollmentId} | Update a tenant employee enrollment |


## create_tenant_employee_enrollment

> <EmptyEnvelope> create_tenant_employee_enrollment(tenant_id, opts)

Create a new tenant employee enrollment

Create a new tenant employee enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_employee_enrollment_create_dto: OpenapiClient::TenantTeamEmployeeEnrollmentCreateDto.new({business_id: 'business_id_example', business_profile_record_id: 'business_profile_record_id_example', business_team_id: 'business_team_id_example', employee_profile_id: 'employee_profile_id_example'}) # TenantTeamEmployeeEnrollmentCreateDto | 
}

begin
  # Create a new tenant employee enrollment
  result = api_instance.create_tenant_employee_enrollment(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->create_tenant_employee_enrollment: #{e}"
end
```

#### Using the create_tenant_employee_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_employee_enrollment_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant employee enrollment
  data, status_code, headers = api_instance.create_tenant_employee_enrollment_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->create_tenant_employee_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_employee_enrollment_create_dto** | [**TenantTeamEmployeeEnrollmentCreateDto**](TenantTeamEmployeeEnrollmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_employee_enrollment

> <EmptyEnvelope> delete_tenant_employee_enrollment(tenant_id, tenant_employee_enrollment_id, opts)

Delete a tenant employee enrollment

Delete a tenant employee enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_employee_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant employee enrollment
  result = api_instance.delete_tenant_employee_enrollment(tenant_id, tenant_employee_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->delete_tenant_employee_enrollment: #{e}"
end
```

#### Using the delete_tenant_employee_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_employee_enrollment_with_http_info(tenant_id, tenant_employee_enrollment_id, opts)

```ruby
begin
  # Delete a tenant employee enrollment
  data, status_code, headers = api_instance.delete_tenant_employee_enrollment_with_http_info(tenant_id, tenant_employee_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->delete_tenant_employee_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_employee_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_employee_enrollment_by_id

> <TenantTeamEmployeeEnrollmentDtoEnvelope> get_tenant_employee_enrollment_by_id(tenant_id, tenant_employee_enrollment_id, opts)

Retrieve a single tenant employee enrollment by its ID

Retrieve a single tenant employee enrollment by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_employee_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant employee enrollment by its ID
  result = api_instance.get_tenant_employee_enrollment_by_id(tenant_id, tenant_employee_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->get_tenant_employee_enrollment_by_id: #{e}"
end
```

#### Using the get_tenant_employee_enrollment_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamEmployeeEnrollmentDtoEnvelope>, Integer, Hash)> get_tenant_employee_enrollment_by_id_with_http_info(tenant_id, tenant_employee_enrollment_id, opts)

```ruby
begin
  # Retrieve a single tenant employee enrollment by its ID
  data, status_code, headers = api_instance.get_tenant_employee_enrollment_by_id_with_http_info(tenant_id, tenant_employee_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamEmployeeEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->get_tenant_employee_enrollment_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_employee_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamEmployeeEnrollmentDtoEnvelope**](TenantTeamEmployeeEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_employee_enrollments

> <TenantTeamEmployeeEnrollmentDtoListEnvelope> get_tenant_employee_enrollments(tenant_id, opts)

Retrieve a list of tenant employee enrollments

Retrieve a list of tenant employee enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant employee enrollments
  result = api_instance.get_tenant_employee_enrollments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->get_tenant_employee_enrollments: #{e}"
end
```

#### Using the get_tenant_employee_enrollments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamEmployeeEnrollmentDtoListEnvelope>, Integer, Hash)> get_tenant_employee_enrollments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant employee enrollments
  data, status_code, headers = api_instance.get_tenant_employee_enrollments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamEmployeeEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->get_tenant_employee_enrollments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamEmployeeEnrollmentDtoListEnvelope**](TenantTeamEmployeeEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_employee_enrollments_count

> <Int32Envelope> get_tenant_employee_enrollments_count(tenant_id, opts)

Get the count of tenant employee enrollments

Get the count of tenant employee enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant employee enrollments
  result = api_instance.get_tenant_employee_enrollments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->get_tenant_employee_enrollments_count: #{e}"
end
```

#### Using the get_tenant_employee_enrollments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_employee_enrollments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant employee enrollments
  data, status_code, headers = api_instance.get_tenant_employee_enrollments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->get_tenant_employee_enrollments_count_with_http_info: #{e}"
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


## update_tenant_employee_enrollment

> <EmptyEnvelope> update_tenant_employee_enrollment(tenant_id, tenant_employee_enrollment_id, opts)

Update a tenant employee enrollment

Update a tenant employee enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::EmployeeEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_employee_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_employee_enrollment_update_dto: OpenapiClient::TenantTeamEmployeeEnrollmentUpdateDto.new # TenantTeamEmployeeEnrollmentUpdateDto | 
}

begin
  # Update a tenant employee enrollment
  result = api_instance.update_tenant_employee_enrollment(tenant_id, tenant_employee_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->update_tenant_employee_enrollment: #{e}"
end
```

#### Using the update_tenant_employee_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_employee_enrollment_with_http_info(tenant_id, tenant_employee_enrollment_id, opts)

```ruby
begin
  # Update a tenant employee enrollment
  data, status_code, headers = api_instance.update_tenant_employee_enrollment_with_http_info(tenant_id, tenant_employee_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EmployeeEnrollmentsApi->update_tenant_employee_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_employee_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_employee_enrollment_update_dto** | [**TenantTeamEmployeeEnrollmentUpdateDto**](TenantTeamEmployeeEnrollmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

