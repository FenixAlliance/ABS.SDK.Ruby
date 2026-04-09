# OpenapiClient::TeamContactEnrollmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_team_contact_enrollment**](TeamContactEnrollmentsApi.md#create_tenant_team_contact_enrollment) | **POST** /api/v2/TenantsService/TeamContactEnrollments | Create a new tenant team contact enrollment |
| [**delete_tenant_team_contact_enrollment**](TeamContactEnrollmentsApi.md#delete_tenant_team_contact_enrollment) | **DELETE** /api/v2/TenantsService/TeamContactEnrollments/{tenantTeamContactEnrollmentId} | Delete a tenant team contact enrollment |
| [**get_tenant_team_contact_enrollment_by_id**](TeamContactEnrollmentsApi.md#get_tenant_team_contact_enrollment_by_id) | **GET** /api/v2/TenantsService/TeamContactEnrollments/{tenantTeamContactEnrollmentId} | Retrieve a single tenant team contact enrollment by its ID |
| [**get_tenant_team_contact_enrollments**](TeamContactEnrollmentsApi.md#get_tenant_team_contact_enrollments) | **GET** /api/v2/TenantsService/TeamContactEnrollments | Retrieve a list of tenant team contact enrollments |
| [**get_tenant_team_contact_enrollments_count**](TeamContactEnrollmentsApi.md#get_tenant_team_contact_enrollments_count) | **GET** /api/v2/TenantsService/TeamContactEnrollments/Count | Get the count of tenant team contact enrollments |
| [**update_tenant_team_contact_enrollment**](TeamContactEnrollmentsApi.md#update_tenant_team_contact_enrollment) | **PUT** /api/v2/TenantsService/TeamContactEnrollments/{tenantTeamContactEnrollmentId} | Update a tenant team contact enrollment |


## create_tenant_team_contact_enrollment

> <EmptyEnvelope> create_tenant_team_contact_enrollment(tenant_id, opts)

Create a new tenant team contact enrollment

Create a new tenant team contact enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamContactEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_contact_enrollment_create_dto: OpenapiClient::TenantTeamContactEnrollmentCreateDto.new({business_id: 'business_id_example', business_profile_record_id: 'business_profile_record_id_example', business_team_id: 'business_team_id_example', contact_id: 'contact_id_example'}) # TenantTeamContactEnrollmentCreateDto | 
}

begin
  # Create a new tenant team contact enrollment
  result = api_instance.create_tenant_team_contact_enrollment(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->create_tenant_team_contact_enrollment: #{e}"
end
```

#### Using the create_tenant_team_contact_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_team_contact_enrollment_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant team contact enrollment
  data, status_code, headers = api_instance.create_tenant_team_contact_enrollment_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->create_tenant_team_contact_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_contact_enrollment_create_dto** | [**TenantTeamContactEnrollmentCreateDto**](TenantTeamContactEnrollmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_team_contact_enrollment

> <EmptyEnvelope> delete_tenant_team_contact_enrollment(tenant_id, tenant_team_contact_enrollment_id, opts)

Delete a tenant team contact enrollment

Delete a tenant team contact enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamContactEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_contact_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant team contact enrollment
  result = api_instance.delete_tenant_team_contact_enrollment(tenant_id, tenant_team_contact_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->delete_tenant_team_contact_enrollment: #{e}"
end
```

#### Using the delete_tenant_team_contact_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_team_contact_enrollment_with_http_info(tenant_id, tenant_team_contact_enrollment_id, opts)

```ruby
begin
  # Delete a tenant team contact enrollment
  data, status_code, headers = api_instance.delete_tenant_team_contact_enrollment_with_http_info(tenant_id, tenant_team_contact_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->delete_tenant_team_contact_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_contact_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_contact_enrollment_by_id

> <TenantTeamContactEnrollmentDtoEnvelope> get_tenant_team_contact_enrollment_by_id(tenant_id, tenant_team_contact_enrollment_id, opts)

Retrieve a single tenant team contact enrollment by its ID

Retrieve a single tenant team contact enrollment by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamContactEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_contact_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant team contact enrollment by its ID
  result = api_instance.get_tenant_team_contact_enrollment_by_id(tenant_id, tenant_team_contact_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->get_tenant_team_contact_enrollment_by_id: #{e}"
end
```

#### Using the get_tenant_team_contact_enrollment_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamContactEnrollmentDtoEnvelope>, Integer, Hash)> get_tenant_team_contact_enrollment_by_id_with_http_info(tenant_id, tenant_team_contact_enrollment_id, opts)

```ruby
begin
  # Retrieve a single tenant team contact enrollment by its ID
  data, status_code, headers = api_instance.get_tenant_team_contact_enrollment_by_id_with_http_info(tenant_id, tenant_team_contact_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamContactEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->get_tenant_team_contact_enrollment_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_contact_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamContactEnrollmentDtoEnvelope**](TenantTeamContactEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_contact_enrollments

> <TenantTeamContactEnrollmentDtoListEnvelope> get_tenant_team_contact_enrollments(tenant_id, opts)

Retrieve a list of tenant team contact enrollments

Retrieve a list of tenant team contact enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamContactEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant team contact enrollments
  result = api_instance.get_tenant_team_contact_enrollments(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->get_tenant_team_contact_enrollments: #{e}"
end
```

#### Using the get_tenant_team_contact_enrollments_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTeamContactEnrollmentDtoListEnvelope>, Integer, Hash)> get_tenant_team_contact_enrollments_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant team contact enrollments
  data, status_code, headers = api_instance.get_tenant_team_contact_enrollments_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTeamContactEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->get_tenant_team_contact_enrollments_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTeamContactEnrollmentDtoListEnvelope**](TenantTeamContactEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_team_contact_enrollments_count

> <Int32Envelope> get_tenant_team_contact_enrollments_count(tenant_id, opts)

Get the count of tenant team contact enrollments

Get the count of tenant team contact enrollments

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamContactEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant team contact enrollments
  result = api_instance.get_tenant_team_contact_enrollments_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->get_tenant_team_contact_enrollments_count: #{e}"
end
```

#### Using the get_tenant_team_contact_enrollments_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_team_contact_enrollments_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant team contact enrollments
  data, status_code, headers = api_instance.get_tenant_team_contact_enrollments_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->get_tenant_team_contact_enrollments_count_with_http_info: #{e}"
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


## update_tenant_team_contact_enrollment

> <EmptyEnvelope> update_tenant_team_contact_enrollment(tenant_id, tenant_team_contact_enrollment_id, opts)

Update a tenant team contact enrollment

Update a tenant team contact enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TeamContactEnrollmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_team_contact_enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_team_contact_enrollment_update_dto: OpenapiClient::TenantTeamContactEnrollmentUpdateDto.new # TenantTeamContactEnrollmentUpdateDto | 
}

begin
  # Update a tenant team contact enrollment
  result = api_instance.update_tenant_team_contact_enrollment(tenant_id, tenant_team_contact_enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->update_tenant_team_contact_enrollment: #{e}"
end
```

#### Using the update_tenant_team_contact_enrollment_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_team_contact_enrollment_with_http_info(tenant_id, tenant_team_contact_enrollment_id, opts)

```ruby
begin
  # Update a tenant team contact enrollment
  data, status_code, headers = api_instance.update_tenant_team_contact_enrollment_with_http_info(tenant_id, tenant_team_contact_enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamContactEnrollmentsApi->update_tenant_team_contact_enrollment_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_team_contact_enrollment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_team_contact_enrollment_update_dto** | [**TenantTeamContactEnrollmentUpdateDto**](TenantTeamContactEnrollmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

