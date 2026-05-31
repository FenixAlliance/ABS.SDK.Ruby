# OpenapiClient::TeamProjectEnrollmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_team_project_enrollment**](TeamProjectEnrollmentsApi.md#create_tenant_team_project_enrollment) | **POST** /api/v2/TenantsService/TeamProjectEnrollments | Create a new tenant team project enrollment |
| [**delete_tenant_team_project_enrollment**](TeamProjectEnrollmentsApi.md#delete_tenant_team_project_enrollment) | **DELETE** /api/v2/TenantsService/TeamProjectEnrollments/{tenantTeamProjectEnrollmentId} | Delete a tenant team project enrollment |
| [**get_tenant_team_project_enrollment_by_id**](TeamProjectEnrollmentsApi.md#get_tenant_team_project_enrollment_by_id) | **GET** /api/v2/TenantsService/TeamProjectEnrollments/{tenantTeamProjectEnrollmentId} | Retrieve a single tenant team project enrollment by its ID |
| [**get_tenant_team_project_enrollments**](TeamProjectEnrollmentsApi.md#get_tenant_team_project_enrollments) | **GET** /api/v2/TenantsService/TeamProjectEnrollments | Retrieve a list of tenant team project enrollments |
| [**get_tenant_team_project_enrollments_count**](TeamProjectEnrollmentsApi.md#get_tenant_team_project_enrollments_count) | **GET** /api/v2/TenantsService/TeamProjectEnrollments/Count | Get the count of tenant team project enrollments |
| [**update_tenant_team_project_enrollment**](TeamProjectEnrollmentsApi.md#update_tenant_team_project_enrollment) | **PUT** /api/v2/TenantsService/TeamProjectEnrollments/{tenantTeamProjectEnrollmentId} | Update a tenant team project enrollment |


## create_tenant_team_project_enrollment

> <EmptyEnvelope> create_tenant_team_project_enrollment(tenant_id, opts)

Create a new tenant team project enrollment

Create a new tenant team project enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamProjectEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_project_enrollment_create_dto: OpenapiClient::TenantTeamProjectEnrollmentCreateDto.new({business_team_id: 'business_team_id_example', project_id: 'project_id_example'}) # TenantTeamProjectEnrollmentCreateDto | 
}

begin
  # Create a new tenant team project enrollment
  result = api_instance.create_tenant_team_project_enrollment(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->create_tenant_team_project_enrollment: #{e}"
end
```

#### Using the create_tenant_team_project_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_team_project_enrollment_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant team project enrollment
  data, status_code, headers = api_instance.create_tenant_team_project_enrollment_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->create_tenant_team_project_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_project_enrollment_create_dto** | [**TenantTeamProjectEnrollmentCreateDto**](TenantTeamProjectEnrollmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_team_project_enrollment

> <EmptyEnvelope> delete_tenant_team_project_enrollment(tenant_id, tenant_team_project_enrollment_id, opts)

Delete a tenant team project enrollment

Delete a tenant team project enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamProjectEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_project_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant team project enrollment
  result = api_instance.delete_tenant_team_project_enrollment(tenant_id, tenant_team_project_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->delete_tenant_team_project_enrollment: #{e}"
end
```

#### Using the delete_tenant_team_project_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_team_project_enrollment_with_http_info(tenant_id, tenant_team_project_enrollment_id, opts)

```ruby
begin
  # Delete a tenant team project enrollment
  data, status_code, headers = api_instance.delete_tenant_team_project_enrollment_with_http_info(tenant_id, tenant_team_project_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->delete_tenant_team_project_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_project_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_project_enrollment_by_id

> <TenantTeamProjectEnrollmentDtoEnvelope> get_tenant_team_project_enrollment_by_id(tenant_id, tenant_team_project_enrollment_id, opts)

Retrieve a single tenant team project enrollment by its ID

Retrieve a single tenant team project enrollment by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamProjectEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_project_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant team project enrollment by its ID
  result = api_instance.get_tenant_team_project_enrollment_by_id(tenant_id, tenant_team_project_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->get_tenant_team_project_enrollment_by_id: #{e}"
end
```

#### Using the get_tenant_team_project_enrollment_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamProjectEnrollmentDtoEnvelope>, Integer, Hash)> get_tenant_team_project_enrollment_by_id_with_http_info(tenant_id, tenant_team_project_enrollment_id, opts)

```ruby
begin
  # Retrieve a single tenant team project enrollment by its ID
  data, status_code, headers = api_instance.get_tenant_team_project_enrollment_by_id_with_http_info(tenant_id, tenant_team_project_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamProjectEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->get_tenant_team_project_enrollment_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_project_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamProjectEnrollmentDtoEnvelope**](TenantTeamProjectEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_project_enrollments

> <TenantTeamProjectEnrollmentDtoListEnvelope> get_tenant_team_project_enrollments(tenant_id, opts)

Retrieve a list of tenant team project enrollments

Retrieve a list of tenant team project enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamProjectEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant team project enrollments
  result = api_instance.get_tenant_team_project_enrollments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->get_tenant_team_project_enrollments: #{e}"
end
```

#### Using the get_tenant_team_project_enrollments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamProjectEnrollmentDtoListEnvelope>, Integer, Hash)> get_tenant_team_project_enrollments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant team project enrollments
  data, status_code, headers = api_instance.get_tenant_team_project_enrollments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamProjectEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->get_tenant_team_project_enrollments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamProjectEnrollmentDtoListEnvelope**](TenantTeamProjectEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_project_enrollments_count

> <Int32Envelope> get_tenant_team_project_enrollments_count(tenant_id, opts)

Get the count of tenant team project enrollments

Get the count of tenant team project enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamProjectEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant team project enrollments
  result = api_instance.get_tenant_team_project_enrollments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->get_tenant_team_project_enrollments_count: #{e}"
end
```

#### Using the get_tenant_team_project_enrollments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_team_project_enrollments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant team project enrollments
  data, status_code, headers = api_instance.get_tenant_team_project_enrollments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->get_tenant_team_project_enrollments_count_with_http_info: #{e}"
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


## update_tenant_team_project_enrollment

> <EmptyEnvelope> update_tenant_team_project_enrollment(tenant_id, tenant_team_project_enrollment_id, opts)

Update a tenant team project enrollment

Update a tenant team project enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamProjectEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_project_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_project_enrollment_update_dto: OpenapiClient::TenantTeamProjectEnrollmentUpdateDto.new # TenantTeamProjectEnrollmentUpdateDto | 
}

begin
  # Update a tenant team project enrollment
  result = api_instance.update_tenant_team_project_enrollment(tenant_id, tenant_team_project_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->update_tenant_team_project_enrollment: #{e}"
end
```

#### Using the update_tenant_team_project_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_team_project_enrollment_with_http_info(tenant_id, tenant_team_project_enrollment_id, opts)

```ruby
begin
  # Update a tenant team project enrollment
  data, status_code, headers = api_instance.update_tenant_team_project_enrollment_with_http_info(tenant_id, tenant_team_project_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamProjectEnrollmentsApi->update_tenant_team_project_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_project_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_project_enrollment_update_dto** | [**TenantTeamProjectEnrollmentUpdateDto**](TenantTeamProjectEnrollmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

