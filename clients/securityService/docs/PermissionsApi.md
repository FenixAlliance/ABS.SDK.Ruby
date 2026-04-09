# OpenapiClient::PermissionsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**assign_permission_to_business_application_async**](PermissionsApi.md#assign_permission_to_business_application_async) | **POST** /api/v2/SecurityService/Permissions/{securityPermissionId}/Applications/{applicationId} | Assign a permission to a business application |
| [**assign_permission_to_enrollment_async**](PermissionsApi.md#assign_permission_to_enrollment_async) | **POST** /api/v2/SecurityService/Permissions/{securityPermissionId}/Enrollments/{enrollmentId} | Assign a permission to an enrollment |
| [**assign_role_to_permission_async**](PermissionsApi.md#assign_role_to_permission_async) | **POST** /api/v2/SecurityService/Permissions/{securityPermissionId}/Roles/{securityRoleId} | Assign a role to a permission |
| [**create_permission_async**](PermissionsApi.md#create_permission_async) | **POST** /api/v2/SecurityService/Permissions | Create a new permission |
| [**delete_permission_async**](PermissionsApi.md#delete_permission_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId} | Delete an existing permission |
| [**get_applications_by_permission_async**](PermissionsApi.md#get_applications_by_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId}/Applications | Get applications by permission |
| [**get_enrollments_by_permission_async**](PermissionsApi.md#get_enrollments_by_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId}/Enrollments | Get enrollments by permission |
| [**get_permission_async**](PermissionsApi.md#get_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId} | Get permission by ID |
| [**get_permissions_async**](PermissionsApi.md#get_permissions_async) | **GET** /api/v2/SecurityService/Permissions | Get all permissions |
| [**get_permissions_by_enrollment_async**](PermissionsApi.md#get_permissions_by_enrollment_async) | **GET** /api/v2/SecurityService/Permissions/ByEnrollment/{enrollmentId} | Get permissions by enrollment |
| [**get_permissions_count_async**](PermissionsApi.md#get_permissions_count_async) | **GET** /api/v2/SecurityService/Permissions/Count | Get permissions count |
| [**get_roles_by_permission_async**](PermissionsApi.md#get_roles_by_permission_async) | **GET** /api/v2/SecurityService/Permissions/{securityPermissionId}/Roles | Get roles by permission |
| [**revoke_permission_from_business_application_async**](PermissionsApi.md#revoke_permission_from_business_application_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId}/Applications/{applicationId} | Revoke a permission from a business application |
| [**revoke_permission_from_enrollment_async**](PermissionsApi.md#revoke_permission_from_enrollment_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId}/Enrollments/{enrollmentId} | Revoke a permission from an enrollment |
| [**revoke_role_from_permission_async**](PermissionsApi.md#revoke_role_from_permission_async) | **DELETE** /api/v2/SecurityService/Permissions/{securityPermissionId}/Roles/{securityRoleId} | Revoke a role from a permission |
| [**update_permission_async**](PermissionsApi.md#update_permission_async) | **PUT** /api/v2/SecurityService/Permissions/{securityPermissionId} | Update an existing permission |


## assign_permission_to_business_application_async

> <EmptyEnvelope> assign_permission_to_business_application_async(tenant_id, security_permission_id, application_id, opts)

Assign a permission to a business application

Assigns a security permission to a business application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a permission to a business application
  result = api_instance.assign_permission_to_business_application_async(tenant_id, security_permission_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->assign_permission_to_business_application_async: #{e}"
end
```

#### Using the assign_permission_to_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_permission_to_business_application_async_with_http_info(tenant_id, security_permission_id, application_id, opts)

```ruby
begin
  # Assign a permission to a business application
  data, status_code, headers = api_instance.assign_permission_to_business_application_async_with_http_info(tenant_id, security_permission_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->assign_permission_to_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## assign_permission_to_enrollment_async

> <EmptyEnvelope> assign_permission_to_enrollment_async(tenant_id, security_permission_id, enrollment_id, opts)

Assign a permission to an enrollment

Assigns a security permission to a tenant enrollment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
enrollment_id = 'enrollment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a permission to an enrollment
  result = api_instance.assign_permission_to_enrollment_async(tenant_id, security_permission_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->assign_permission_to_enrollment_async: #{e}"
end
```

#### Using the assign_permission_to_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_permission_to_enrollment_async_with_http_info(tenant_id, security_permission_id, enrollment_id, opts)

```ruby
begin
  # Assign a permission to an enrollment
  data, status_code, headers = api_instance.assign_permission_to_enrollment_async_with_http_info(tenant_id, security_permission_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->assign_permission_to_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
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


## assign_role_to_permission_async

> <EmptyEnvelope> assign_role_to_permission_async(tenant_id, security_permission_id, security_role_id, opts)

Assign a role to a permission

Assigns a security role to a security permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a role to a permission
  result = api_instance.assign_role_to_permission_async(tenant_id, security_permission_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->assign_role_to_permission_async: #{e}"
end
```

#### Using the assign_role_to_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_role_to_permission_async_with_http_info(tenant_id, security_permission_id, security_role_id, opts)

```ruby
begin
  # Assign a role to a permission
  data, status_code, headers = api_instance.assign_role_to_permission_async_with_http_info(tenant_id, security_permission_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->assign_role_to_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_permission_async

> <EmptyEnvelope> create_permission_async(tenant_id, security_permission_create_dto, opts)

Create a new permission

Creates a new security permission for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_create_dto = OpenapiClient::SecurityPermissionCreateDto.new({name: 'name_example', tenant_id: 'tenant_id_example'}) # SecurityPermissionCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a new permission
  result = api_instance.create_permission_async(tenant_id, security_permission_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->create_permission_async: #{e}"
end
```

#### Using the create_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_permission_async_with_http_info(tenant_id, security_permission_create_dto, opts)

```ruby
begin
  # Create a new permission
  data, status_code, headers = api_instance.create_permission_async_with_http_info(tenant_id, security_permission_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->create_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_create_dto** | [**SecurityPermissionCreateDto**](SecurityPermissionCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_permission_async

> <EmptyEnvelope> delete_permission_async(tenant_id, security_permission_id, opts)

Delete an existing permission

Deletes an existing security permission for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an existing permission
  result = api_instance.delete_permission_async(tenant_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->delete_permission_async: #{e}"
end
```

#### Using the delete_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_permission_async_with_http_info(tenant_id, security_permission_id, opts)

```ruby
begin
  # Delete an existing permission
  data, status_code, headers = api_instance.delete_permission_async_with_http_info(tenant_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->delete_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_applications_by_permission_async

> <BusinessApplicationSimpleDtoListEnvelope> get_applications_by_permission_async(tenant_id, security_permission_id, opts)

Get applications by permission

Retrieves all business applications that have a specific permission granted.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get applications by permission
  result = api_instance.get_applications_by_permission_async(tenant_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_applications_by_permission_async: #{e}"
end
```

#### Using the get_applications_by_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessApplicationSimpleDtoListEnvelope>, Integer, Hash)> get_applications_by_permission_async_with_http_info(tenant_id, security_permission_id, opts)

```ruby
begin
  # Get applications by permission
  data, status_code, headers = api_instance.get_applications_by_permission_async_with_http_info(tenant_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessApplicationSimpleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_applications_by_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessApplicationSimpleDtoListEnvelope**](BusinessApplicationSimpleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollments_by_permission_async

> <TenantEnrollmentDtoListEnvelope> get_enrollments_by_permission_async(tenant_id, security_permission_id, opts)

Get enrollments by permission

Retrieves all tenant enrollments that have a specific permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get enrollments by permission
  result = api_instance.get_enrollments_by_permission_async(tenant_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_enrollments_by_permission_async: #{e}"
end
```

#### Using the get_enrollments_by_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_enrollments_by_permission_async_with_http_info(tenant_id, security_permission_id, opts)

```ruby
begin
  # Get enrollments by permission
  data, status_code, headers = api_instance.get_enrollments_by_permission_async_with_http_info(tenant_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_enrollments_by_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_permission_async

> <SecurityPermissionDtoEnvelope> get_permission_async(tenant_id, security_permission_id, opts)

Get permission by ID

Retrieves a specific security permission by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get permission by ID
  result = api_instance.get_permission_async(tenant_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permission_async: #{e}"
end
```

#### Using the get_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityPermissionDtoEnvelope>, Integer, Hash)> get_permission_async_with_http_info(tenant_id, security_permission_id, opts)

```ruby
begin
  # Get permission by ID
  data, status_code, headers = api_instance.get_permission_async_with_http_info(tenant_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityPermissionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityPermissionDtoEnvelope**](SecurityPermissionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_permissions_async

> <SecurityPermissionDtoListEnvelope> get_permissions_async(tenant_id, opts)

Get all permissions

Retrieves all security permissions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all permissions
  result = api_instance.get_permissions_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permissions_async: #{e}"
end
```

#### Using the get_permissions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityPermissionDtoListEnvelope>, Integer, Hash)> get_permissions_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all permissions
  data, status_code, headers = api_instance.get_permissions_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityPermissionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permissions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityPermissionDtoListEnvelope**](SecurityPermissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_permissions_by_enrollment_async

> <SecurityPermissionDtoListEnvelope> get_permissions_by_enrollment_async(tenant_id, enrollment_id, opts)

Get permissions by enrollment

Retrieves all security permissions granted to a specific enrollment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = 'enrollment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get permissions by enrollment
  result = api_instance.get_permissions_by_enrollment_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permissions_by_enrollment_async: #{e}"
end
```

#### Using the get_permissions_by_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityPermissionDtoListEnvelope>, Integer, Hash)> get_permissions_by_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get permissions by enrollment
  data, status_code, headers = api_instance.get_permissions_by_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityPermissionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permissions_by_enrollment_async_with_http_info: #{e}"
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

[**SecurityPermissionDtoListEnvelope**](SecurityPermissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_permissions_count_async

> <Int32Envelope> get_permissions_count_async(tenant_id, opts)

Get permissions count

Retrieves the count of security permissions for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get permissions count
  result = api_instance.get_permissions_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permissions_count_async: #{e}"
end
```

#### Using the get_permissions_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_permissions_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get permissions count
  data, status_code, headers = api_instance.get_permissions_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_permissions_count_async_with_http_info: #{e}"
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


## get_roles_by_permission_async

> <SecurityRoleDtoListEnvelope> get_roles_by_permission_async(tenant_id, security_permission_id, opts)

Get roles by permission

Retrieves all security roles that have a specific permission granted.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get roles by permission
  result = api_instance.get_roles_by_permission_async(tenant_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_roles_by_permission_async: #{e}"
end
```

#### Using the get_roles_by_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityRoleDtoListEnvelope>, Integer, Hash)> get_roles_by_permission_async_with_http_info(tenant_id, security_permission_id, opts)

```ruby
begin
  # Get roles by permission
  data, status_code, headers = api_instance.get_roles_by_permission_async_with_http_info(tenant_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityRoleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->get_roles_by_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityRoleDtoListEnvelope**](SecurityRoleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## revoke_permission_from_business_application_async

> <EmptyEnvelope> revoke_permission_from_business_application_async(tenant_id, security_permission_id, application_id, opts)

Revoke a permission from a business application

Revokes a security permission from a business application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
application_id = 'application_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a permission from a business application
  result = api_instance.revoke_permission_from_business_application_async(tenant_id, security_permission_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->revoke_permission_from_business_application_async: #{e}"
end
```

#### Using the revoke_permission_from_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_permission_from_business_application_async_with_http_info(tenant_id, security_permission_id, application_id, opts)

```ruby
begin
  # Revoke a permission from a business application
  data, status_code, headers = api_instance.revoke_permission_from_business_application_async_with_http_info(tenant_id, security_permission_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->revoke_permission_from_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **application_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## revoke_permission_from_enrollment_async

> <EmptyEnvelope> revoke_permission_from_enrollment_async(tenant_id, security_permission_id, enrollment_id, opts)

Revoke a permission from an enrollment

Revokes a security permission from a tenant enrollment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
enrollment_id = 'enrollment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a permission from an enrollment
  result = api_instance.revoke_permission_from_enrollment_async(tenant_id, security_permission_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->revoke_permission_from_enrollment_async: #{e}"
end
```

#### Using the revoke_permission_from_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_permission_from_enrollment_async_with_http_info(tenant_id, security_permission_id, enrollment_id, opts)

```ruby
begin
  # Revoke a permission from an enrollment
  data, status_code, headers = api_instance.revoke_permission_from_enrollment_async_with_http_info(tenant_id, security_permission_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->revoke_permission_from_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
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


## revoke_role_from_permission_async

> <EmptyEnvelope> revoke_role_from_permission_async(tenant_id, security_permission_id, security_role_id, opts)

Revoke a role from a permission

Revokes a security role from a security permission.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a role from a permission
  result = api_instance.revoke_role_from_permission_async(tenant_id, security_permission_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->revoke_role_from_permission_async: #{e}"
end
```

#### Using the revoke_role_from_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_role_from_permission_async_with_http_info(tenant_id, security_permission_id, security_role_id, opts)

```ruby
begin
  # Revoke a role from a permission
  data, status_code, headers = api_instance.revoke_role_from_permission_async_with_http_info(tenant_id, security_permission_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->revoke_role_from_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_permission_async

> <EmptyEnvelope> update_permission_async(tenant_id, security_permission_id, security_permission_update_dto, opts)

Update an existing permission

Updates an existing security permission for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PermissionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_permission_id = 'security_permission_id_example' # String | 
security_permission_update_dto = OpenapiClient::SecurityPermissionUpdateDto.new({name: 'name_example'}) # SecurityPermissionUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an existing permission
  result = api_instance.update_permission_async(tenant_id, security_permission_id, security_permission_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->update_permission_async: #{e}"
end
```

#### Using the update_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_permission_async_with_http_info(tenant_id, security_permission_id, security_permission_update_dto, opts)

```ruby
begin
  # Update an existing permission
  data, status_code, headers = api_instance.update_permission_async_with_http_info(tenant_id, security_permission_id, security_permission_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PermissionsApi->update_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_permission_id** | **String** |  |  |
| **security_permission_update_dto** | [**SecurityPermissionUpdateDto**](SecurityPermissionUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

