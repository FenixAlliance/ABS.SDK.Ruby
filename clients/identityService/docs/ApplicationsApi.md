# OpenapiClient::ApplicationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_application**](ApplicationsApi.md#get_application) | **GET** /api/v2/Applications/{appId} | Get application by ID |
| [**get_granted_enrollment_permissions**](ApplicationsApi.md#get_granted_enrollment_permissions) | **GET** /api/v2/Applications/{appId}/GrantedRoles/{securityRoleId}/GrantedPermissions | Get granted permissions for an application role |
| [**get_granted_tenant_permissions**](ApplicationsApi.md#get_granted_tenant_permissions) | **GET** /api/v2/Applications/{appId}/GrantedPermissions | Get granted tenant permissions for an application |
| [**get_granted_tenant_roles**](ApplicationsApi.md#get_granted_tenant_roles) | **GET** /api/v2/Applications/{appId}/GrantedRoles | Get granted tenant roles for an application |
| [**get_required_permissions**](ApplicationsApi.md#get_required_permissions) | **GET** /api/v2/Applications/{appId}/RequiredPermissions | Get required permissions for an application |


## get_application

> get_application(app_id, opts)

Get application by ID

Retrieves an application by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
app_id = 'app_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get application by ID
  api_instance.get_application(app_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_application: #{e}"
end
```

#### Using the get_application_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_application_with_http_info(app_id, opts)

```ruby
begin
  # Get application by ID
  data, status_code, headers = api_instance.get_application_with_http_info(app_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_application_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **app_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## get_granted_enrollment_permissions

> get_granted_enrollment_permissions(app_id, security_role_id, opts)

Get granted permissions for an application role

Retrieves the list of permissions granted through a specific security role for the specified application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
app_id = 'app_id_example' # String | 
security_role_id = 'security_role_id_example' # String | 
opts = {
  enrollment_id: 'enrollment_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get granted permissions for an application role
  api_instance.get_granted_enrollment_permissions(app_id, security_role_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_granted_enrollment_permissions: #{e}"
end
```

#### Using the get_granted_enrollment_permissions_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_granted_enrollment_permissions_with_http_info(app_id, security_role_id, opts)

```ruby
begin
  # Get granted permissions for an application role
  data, status_code, headers = api_instance.get_granted_enrollment_permissions_with_http_info(app_id, security_role_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_granted_enrollment_permissions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **app_id** | **String** |  |  |
| **security_role_id** | **String** |  |  |
| **enrollment_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## get_granted_tenant_permissions

> get_granted_tenant_permissions(app_id, opts)

Get granted tenant permissions for an application

Retrieves the list of permissions granted to the specified application within a tenant context.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
app_id = 'app_id_example' # String | 
opts = {
  tenant_id: 'tenant_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get granted tenant permissions for an application
  api_instance.get_granted_tenant_permissions(app_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_granted_tenant_permissions: #{e}"
end
```

#### Using the get_granted_tenant_permissions_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_granted_tenant_permissions_with_http_info(app_id, opts)

```ruby
begin
  # Get granted tenant permissions for an application
  data, status_code, headers = api_instance.get_granted_tenant_permissions_with_http_info(app_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_granted_tenant_permissions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **app_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## get_granted_tenant_roles

> get_granted_tenant_roles(app_id, opts)

Get granted tenant roles for an application

Retrieves the list of security roles granted to the specified application within a tenant context.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
app_id = 'app_id_example' # String | 
opts = {
  tenant_id: 'tenant_id_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get granted tenant roles for an application
  api_instance.get_granted_tenant_roles(app_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_granted_tenant_roles: #{e}"
end
```

#### Using the get_granted_tenant_roles_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_granted_tenant_roles_with_http_info(app_id, opts)

```ruby
begin
  # Get granted tenant roles for an application
  data, status_code, headers = api_instance.get_granted_tenant_roles_with_http_info(app_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_granted_tenant_roles_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **app_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## get_required_permissions

> get_required_permissions(app_id, opts)

Get required permissions for an application

Retrieves the list of permissions required by the specified application.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationsApi.new
app_id = 'app_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get required permissions for an application
  api_instance.get_required_permissions(app_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_required_permissions: #{e}"
end
```

#### Using the get_required_permissions_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_required_permissions_with_http_info(app_id, opts)

```ruby
begin
  # Get required permissions for an application
  data, status_code, headers = api_instance.get_required_permissions_with_http_info(app_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationsApi->get_required_permissions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **app_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

