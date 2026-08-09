# OpenapiClient::RolesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**assign_permission_to_role_async**](RolesApi.md#assign_permission_to_role_async) | **POST** /api/v2/SecurityService/Roles/{securityRoleId}/Permissions/{securityPermissionId} | Assign a permission to a role |
| [**assign_role_to_business_application_async**](RolesApi.md#assign_role_to_business_application_async) | **POST** /api/v2/SecurityService/Roles/{securityRoleId}/Applications/{applicationId} | Assign a role to a business application |
| [**assign_role_to_enrollment_async**](RolesApi.md#assign_role_to_enrollment_async) | **POST** /api/v2/SecurityService/Roles/{securityRoleId}/Enrollments/{enrollmentId} | Assign a role to an enrollment |
| [**create_role_async**](RolesApi.md#create_role_async) | **POST** /api/v2/SecurityService/Roles | Create a new role |
| [**delete_role_async**](RolesApi.md#delete_role_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId} | Delete an existing role |
| [**get_applications_by_role_async**](RolesApi.md#get_applications_by_role_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId}/Applications | Get applications by role |
| [**get_enrollments_by_role_async**](RolesApi.md#get_enrollments_by_role_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId}/Enrollments | Get enrollments by role |
| [**get_role_async**](RolesApi.md#get_role_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId} | Get role by ID |
| [**get_role_permissions_async**](RolesApi.md#get_role_permissions_async) | **GET** /api/v2/SecurityService/Roles/{securityRoleId}/Permissions | Get permissions by role |
| [**get_roles_async**](RolesApi.md#get_roles_async) | **GET** /api/v2/SecurityService/Roles | Get all roles |
| [**get_roles_by_enrollment_async**](RolesApi.md#get_roles_by_enrollment_async) | **GET** /api/v2/SecurityService/Roles/ByEnrollment/{enrollmentId} | Get roles by enrollment |
| [**get_roles_count_async**](RolesApi.md#get_roles_count_async) | **GET** /api/v2/SecurityService/Roles/Count | Get roles count |
| [**patch_role_async**](RolesApi.md#patch_role_async) | **PATCH** /api/v2/SecurityService/Roles/{securityRoleId} | Patch an existing role |
| [**revoke_permission_from_role_async**](RolesApi.md#revoke_permission_from_role_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId}/Permissions/{securityPermissionId} | Revoke a permission from a role |
| [**revoke_role_from_business_application_async**](RolesApi.md#revoke_role_from_business_application_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId}/Applications/{applicationId} | Revoke a role from a business application |
| [**revoke_role_from_enrollment_async**](RolesApi.md#revoke_role_from_enrollment_async) | **DELETE** /api/v2/SecurityService/Roles/{securityRoleId}/Enrollments/{enrollmentId} | Revoke a role from an enrollment |
| [**update_role_async**](RolesApi.md#update_role_async) | **PUT** /api/v2/SecurityService/Roles/{securityRoleId} | Update an existing role |


## assign_permission_to_role_async

> <EmptyEnvelope> assign_permission_to_role_async(tenant_id, security_role_id, security_permission_id, opts)

Assign a permission to a role

Assigns a security permission to a security role.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a permission to a role
  result = api_instance.assign_permission_to_role_async(tenant_id, security_role_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->assign_permission_to_role_async: #{e}"
end
```

#### Using the assign_permission_to_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_permission_to_role_async_with_http_info(tenant_id, security_role_id, security_permission_id, opts)

```ruby
begin
  # Assign a permission to a role
  data, status_code, headers = api_instance.assign_permission_to_role_async_with_http_info(tenant_id, security_role_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->assign_permission_to_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
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


## assign_role_to_business_application_async

> <EmptyEnvelope> assign_role_to_business_application_async(tenant_id, security_role_id, application_id, opts)

Assign a role to a business application

Assigns a security role to a business application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a role to a business application
  result = api_instance.assign_role_to_business_application_async(tenant_id, security_role_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->assign_role_to_business_application_async: #{e}"
end
```

#### Using the assign_role_to_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_role_to_business_application_async_with_http_info(tenant_id, security_role_id, application_id, opts)

```ruby
begin
  # Assign a role to a business application
  data, status_code, headers = api_instance.assign_role_to_business_application_async_with_http_info(tenant_id, security_role_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->assign_role_to_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
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


## assign_role_to_enrollment_async

> <EmptyEnvelope> assign_role_to_enrollment_async(tenant_id, security_role_id, enrollment_id, opts)

Assign a role to an enrollment

Assigns a security role to a tenant enrollment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
enrollment_id = 'enrollment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a role to an enrollment
  result = api_instance.assign_role_to_enrollment_async(tenant_id, security_role_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->assign_role_to_enrollment_async: #{e}"
end
```

#### Using the assign_role_to_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> assign_role_to_enrollment_async_with_http_info(tenant_id, security_role_id, enrollment_id, opts)

```ruby
begin
  # Assign a role to an enrollment
  data, status_code, headers = api_instance.assign_role_to_enrollment_async_with_http_info(tenant_id, security_role_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->assign_role_to_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
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


## create_role_async

> <EmptyEnvelope> create_role_async(tenant_id, security_role_create_dto, opts)

Create a new role

Creates a new security role for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_create_dto = OpenapiClient::SecurityRoleCreateDto.new({name: 'name_example'}) # SecurityRoleCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a new role
  result = api_instance.create_role_async(tenant_id, security_role_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->create_role_async: #{e}"
end
```

#### Using the create_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_role_async_with_http_info(tenant_id, security_role_create_dto, opts)

```ruby
begin
  # Create a new role
  data, status_code, headers = api_instance.create_role_async_with_http_info(tenant_id, security_role_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->create_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_create_dto** | [**SecurityRoleCreateDto**](SecurityRoleCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_role_async

> <EmptyEnvelope> delete_role_async(tenant_id, security_role_id, opts)

Delete an existing role

Deletes an existing security role for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an existing role
  result = api_instance.delete_role_async(tenant_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->delete_role_async: #{e}"
end
```

#### Using the delete_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_role_async_with_http_info(tenant_id, security_role_id, opts)

```ruby
begin
  # Delete an existing role
  data, status_code, headers = api_instance.delete_role_async_with_http_info(tenant_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->delete_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## get_applications_by_role_async

> <BusinessApplicationSimpleDtoListEnvelope> get_applications_by_role_async(tenant_id, security_role_id, opts)

Get applications by role

Retrieves all business applications that have a specific role granted.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get applications by role
  result = api_instance.get_applications_by_role_async(tenant_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_applications_by_role_async: #{e}"
end
```

#### Using the get_applications_by_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BusinessApplicationSimpleDtoListEnvelope>, Integer, Hash)> get_applications_by_role_async_with_http_info(tenant_id, security_role_id, opts)

```ruby
begin
  # Get applications by role
  data, status_code, headers = api_instance.get_applications_by_role_async_with_http_info(tenant_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BusinessApplicationSimpleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_applications_by_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BusinessApplicationSimpleDtoListEnvelope**](BusinessApplicationSimpleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollments_by_role_async

> <TenantEnrollmentDtoListEnvelope> get_enrollments_by_role_async(tenant_id, security_role_id, opts)

Get enrollments by role

Retrieves all tenant enrollments that have a specific role.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get enrollments by role
  result = api_instance.get_enrollments_by_role_async(tenant_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_enrollments_by_role_async: #{e}"
end
```

#### Using the get_enrollments_by_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_enrollments_by_role_async_with_http_info(tenant_id, security_role_id, opts)

```ruby
begin
  # Get enrollments by role
  data, status_code, headers = api_instance.get_enrollments_by_role_async_with_http_info(tenant_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_enrollments_by_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantEnrollmentDtoListEnvelope**](TenantEnrollmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_role_async

> <SecurityRoleDtoEnvelope> get_role_async(tenant_id, security_role_id, opts)

Get role by ID

Retrieves a specific security role by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get role by ID
  result = api_instance.get_role_async(tenant_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_role_async: #{e}"
end
```

#### Using the get_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityRoleDtoEnvelope>, Integer, Hash)> get_role_async_with_http_info(tenant_id, security_role_id, opts)

```ruby
begin
  # Get role by ID
  data, status_code, headers = api_instance.get_role_async_with_http_info(tenant_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityRoleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityRoleDtoEnvelope**](SecurityRoleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_role_permissions_async

> <SecurityPermissionDtoListEnvelope> get_role_permissions_async(tenant_id, security_role_id, opts)

Get permissions by role

Retrieves all security permissions assigned to a specific role.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get permissions by role
  result = api_instance.get_role_permissions_async(tenant_id, security_role_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_role_permissions_async: #{e}"
end
```

#### Using the get_role_permissions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityPermissionDtoListEnvelope>, Integer, Hash)> get_role_permissions_async_with_http_info(tenant_id, security_role_id, opts)

```ruby
begin
  # Get permissions by role
  data, status_code, headers = api_instance.get_role_permissions_async_with_http_info(tenant_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityPermissionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_role_permissions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SecurityPermissionDtoListEnvelope**](SecurityPermissionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_roles_async

> <SecurityRoleDtoListEnvelope> get_roles_async(tenant_id, opts)

Get all roles

Retrieves all security roles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  security_role_dto_collection_query_parameters: OpenapiClient::SecurityRoleDtoCollectionQueryParameters.new # SecurityRoleDtoCollectionQueryParameters | 
}

begin
  # Get all roles
  result = api_instance.get_roles_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_roles_async: #{e}"
end
```

#### Using the get_roles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityRoleDtoListEnvelope>, Integer, Hash)> get_roles_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all roles
  data, status_code, headers = api_instance.get_roles_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityRoleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_roles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **security_role_dto_collection_query_parameters** | [**SecurityRoleDtoCollectionQueryParameters**](SecurityRoleDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SecurityRoleDtoListEnvelope**](SecurityRoleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_roles_by_enrollment_async

> <SecurityRoleDtoListEnvelope> get_roles_by_enrollment_async(tenant_id, enrollment_id, opts)

Get roles by enrollment

Retrieves all security roles granted to a specific enrollment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = 'enrollment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get roles by enrollment
  result = api_instance.get_roles_by_enrollment_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_roles_by_enrollment_async: #{e}"
end
```

#### Using the get_roles_by_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityRoleDtoListEnvelope>, Integer, Hash)> get_roles_by_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get roles by enrollment
  data, status_code, headers = api_instance.get_roles_by_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityRoleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_roles_by_enrollment_async_with_http_info: #{e}"
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

[**SecurityRoleDtoListEnvelope**](SecurityRoleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_roles_count_async

> <Int32Envelope> get_roles_count_async(tenant_id, opts)

Get roles count

Retrieves the count of security roles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  security_role_dto_collection_query_parameters: OpenapiClient::SecurityRoleDtoCollectionQueryParameters.new # SecurityRoleDtoCollectionQueryParameters | 
}

begin
  # Get roles count
  result = api_instance.get_roles_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_roles_count_async: #{e}"
end
```

#### Using the get_roles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_roles_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get roles count
  data, status_code, headers = api_instance.get_roles_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->get_roles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **security_role_dto_collection_query_parameters** | [**SecurityRoleDtoCollectionQueryParameters**](SecurityRoleDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_role_async

> <EmptyEnvelope> patch_role_async(tenant_id, security_role_id, patch_operation, opts)

Patch an existing role

Partially updates an existing security role using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
patch_operation = [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Patch an existing role
  result = api_instance.patch_role_async(tenant_id, security_role_id, patch_operation, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->patch_role_async: #{e}"
end
```

#### Using the patch_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_role_async_with_http_info(tenant_id, security_role_id, patch_operation, opts)

```ruby
begin
  # Patch an existing role
  data, status_code, headers = api_instance.patch_role_async_with_http_info(tenant_id, security_role_id, patch_operation, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->patch_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## revoke_permission_from_role_async

> <EmptyEnvelope> revoke_permission_from_role_async(tenant_id, security_role_id, security_permission_id, opts)

Revoke a permission from a role

Revokes a security permission from a security role.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
security_permission_id = 'security_permission_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a permission from a role
  result = api_instance.revoke_permission_from_role_async(tenant_id, security_role_id, security_permission_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->revoke_permission_from_role_async: #{e}"
end
```

#### Using the revoke_permission_from_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_permission_from_role_async_with_http_info(tenant_id, security_role_id, security_permission_id, opts)

```ruby
begin
  # Revoke a permission from a role
  data, status_code, headers = api_instance.revoke_permission_from_role_async_with_http_info(tenant_id, security_role_id, security_permission_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->revoke_permission_from_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
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


## revoke_role_from_business_application_async

> <EmptyEnvelope> revoke_role_from_business_application_async(tenant_id, security_role_id, application_id, opts)

Revoke a role from a business application

Revokes a security role from a business application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
application_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a role from a business application
  result = api_instance.revoke_role_from_business_application_async(tenant_id, security_role_id, application_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->revoke_role_from_business_application_async: #{e}"
end
```

#### Using the revoke_role_from_business_application_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_role_from_business_application_async_with_http_info(tenant_id, security_role_id, application_id, opts)

```ruby
begin
  # Revoke a role from a business application
  data, status_code, headers = api_instance.revoke_role_from_business_application_async_with_http_info(tenant_id, security_role_id, application_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->revoke_role_from_business_application_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
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


## revoke_role_from_enrollment_async

> <EmptyEnvelope> revoke_role_from_enrollment_async(tenant_id, security_role_id, enrollment_id, opts)

Revoke a role from an enrollment

Revokes a security role from a tenant enrollment.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
enrollment_id = 'enrollment_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a role from an enrollment
  result = api_instance.revoke_role_from_enrollment_async(tenant_id, security_role_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->revoke_role_from_enrollment_async: #{e}"
end
```

#### Using the revoke_role_from_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_role_from_enrollment_async_with_http_info(tenant_id, security_role_id, enrollment_id, opts)

```ruby
begin
  # Revoke a role from an enrollment
  data, status_code, headers = api_instance.revoke_role_from_enrollment_async_with_http_info(tenant_id, security_role_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->revoke_role_from_enrollment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
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


## update_role_async

> <EmptyEnvelope> update_role_async(tenant_id, security_role_id, security_role_update_dto, opts)

Update an existing role

Updates an existing security role for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RolesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
security_role_id = 'security_role_id_example' # String | 
security_role_update_dto = OpenapiClient::SecurityRoleUpdateDto.new({name: 'name_example'}) # SecurityRoleUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update an existing role
  result = api_instance.update_role_async(tenant_id, security_role_id, security_role_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->update_role_async: #{e}"
end
```

#### Using the update_role_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_role_async_with_http_info(tenant_id, security_role_id, security_role_update_dto, opts)

```ruby
begin
  # Update an existing role
  data, status_code, headers = api_instance.update_role_async_with_http_info(tenant_id, security_role_id, security_role_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RolesApi->update_role_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **security_role_update_dto** | [**SecurityRoleUpdateDto**](SecurityRoleUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

