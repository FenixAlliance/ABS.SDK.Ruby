# OpenapiClient::ApplicationPrincipalsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**disable_application_principal_async**](ApplicationPrincipalsApi.md#disable_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Disable | Disable an application principal |
| [**enable_application_principal_async**](ApplicationPrincipalsApi.md#enable_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Enable | Enable an application principal |
| [**get_application_principal_async**](ApplicationPrincipalsApi.md#get_application_principal_async) | **GET** /api/v2/SecurityService/ApplicationPrincipals/{principalId} | Get application principal by ID |
| [**get_application_principals_async**](ApplicationPrincipalsApi.md#get_application_principals_async) | **GET** /api/v2/SecurityService/ApplicationPrincipals | Get all application principals |
| [**get_application_principals_count_async**](ApplicationPrincipalsApi.md#get_application_principals_count_async) | **GET** /api/v2/SecurityService/ApplicationPrincipals/Count | Get application principals count |
| [**grant_permission_async**](ApplicationPrincipalsApi.md#grant_permission_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Permissions | Grant a permission to an application principal |
| [**provision_application_principal_async**](ApplicationPrincipalsApi.md#provision_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/Provision | Provision an application principal |
| [**revoke_permission_async**](ApplicationPrincipalsApi.md#revoke_permission_async) | **DELETE** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Permissions/{permission} | Revoke a permission from an application principal |
| [**suspend_application_principal_async**](ApplicationPrincipalsApi.md#suspend_application_principal_async) | **POST** /api/v2/SecurityService/ApplicationPrincipals/{principalId}/Suspend | Suspend an application principal |


## disable_application_principal_async

> <EmptyEnvelope> disable_application_principal_async(tenant_id, principal_id, opts)

Disable an application principal

Disables the application principal; dependent unattended execution fails closed.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Disable an application principal
  result = api_instance.disable_application_principal_async(tenant_id, principal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->disable_application_principal_async: #{e}"
end
```

#### Using the disable_application_principal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> disable_application_principal_async_with_http_info(tenant_id, principal_id, opts)

```ruby
begin
  # Disable an application principal
  data, status_code, headers = api_instance.disable_application_principal_async_with_http_info(tenant_id, principal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->disable_application_principal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **principal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## enable_application_principal_async

> <EmptyEnvelope> enable_application_principal_async(tenant_id, principal_id, opts)

Enable an application principal

Reinstates the application principal to the Active lifecycle state.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Enable an application principal
  result = api_instance.enable_application_principal_async(tenant_id, principal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->enable_application_principal_async: #{e}"
end
```

#### Using the enable_application_principal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> enable_application_principal_async_with_http_info(tenant_id, principal_id, opts)

```ruby
begin
  # Enable an application principal
  data, status_code, headers = api_instance.enable_application_principal_async_with_http_info(tenant_id, principal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->enable_application_principal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **principal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_application_principal_async

> <ApplicationPrincipalDetailDtoEnvelope> get_application_principal_async(tenant_id, principal_id, opts)

Get application principal by ID

Retrieves a specific application principal: owning application, tenant enrollment, lifecycle status, system-locked flag, and its explicit least-privilege permission grants.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get application principal by ID
  result = api_instance.get_application_principal_async(tenant_id, principal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_application_principal_async: #{e}"
end
```

#### Using the get_application_principal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalDetailDtoEnvelope>, Integer, Hash)> get_application_principal_async_with_http_info(tenant_id, principal_id, opts)

```ruby
begin
  # Get application principal by ID
  data, status_code, headers = api_instance.get_application_principal_async_with_http_info(tenant_id, principal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalDetailDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_application_principal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **principal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ApplicationPrincipalDetailDtoEnvelope**](ApplicationPrincipalDetailDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_application_principals_async

> <ApplicationPrincipalDtoListEnvelope> get_application_principals_async(tenant_id, opts)

Get all application principals

Retrieves the non-human application principals enrolled in the specified tenant (including read-only system-locked platform principals).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  application_principal_dto_collection_query_parameters: OpenapiClient::ApplicationPrincipalDtoCollectionQueryParameters.new # ApplicationPrincipalDtoCollectionQueryParameters | 
}

begin
  # Get all application principals
  result = api_instance.get_application_principals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_application_principals_async: #{e}"
end
```

#### Using the get_application_principals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalDtoListEnvelope>, Integer, Hash)> get_application_principals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all application principals
  data, status_code, headers = api_instance.get_application_principals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_application_principals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **application_principal_dto_collection_query_parameters** | [**ApplicationPrincipalDtoCollectionQueryParameters**](ApplicationPrincipalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ApplicationPrincipalDtoListEnvelope**](ApplicationPrincipalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_application_principals_count_async

> <Int32Envelope> get_application_principals_count_async(tenant_id, opts)

Get application principals count

Retrieves the count of application principals enrolled in the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  application_principal_dto_collection_query_parameters: OpenapiClient::ApplicationPrincipalDtoCollectionQueryParameters.new # ApplicationPrincipalDtoCollectionQueryParameters | 
}

begin
  # Get application principals count
  result = api_instance.get_application_principals_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_application_principals_count_async: #{e}"
end
```

#### Using the get_application_principals_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_application_principals_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get application principals count
  data, status_code, headers = api_instance.get_application_principals_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_application_principals_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **application_principal_dto_collection_query_parameters** | [**ApplicationPrincipalDtoCollectionQueryParameters**](ApplicationPrincipalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## grant_permission_async

> <EmptyEnvelope> grant_permission_async(tenant_id, principal_id, application_principal_permission_request_dto, opts)

Grant a permission to an application principal

Grants a single least-privilege permission to the application principal's enrollment. Owner/admin/wildcard/*_manage permissions are rejected; system-locked principals require a platform administrator.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_principal_permission_request_dto = OpenapiClient::ApplicationPrincipalPermissionRequestDto.new({permission: 'permission_example'}) # ApplicationPrincipalPermissionRequestDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Grant a permission to an application principal
  result = api_instance.grant_permission_async(tenant_id, principal_id, application_principal_permission_request_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->grant_permission_async: #{e}"
end
```

#### Using the grant_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> grant_permission_async_with_http_info(tenant_id, principal_id, application_principal_permission_request_dto, opts)

```ruby
begin
  # Grant a permission to an application principal
  data, status_code, headers = api_instance.grant_permission_async_with_http_info(tenant_id, principal_id, application_principal_permission_request_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->grant_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **principal_id** | **String** |  |  |
| **application_principal_permission_request_dto** | [**ApplicationPrincipalPermissionRequestDto**](ApplicationPrincipalPermissionRequestDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## provision_application_principal_async

> <ApplicationPrincipalProvisioningResultDtoEnvelope> provision_application_principal_async(tenant_id, application_principal_provision_request_dto, opts)

Provision an application principal

Idempotently provisions the application principal (and its own least-privilege enrollment) for a governed business application in the specified tenant. System-locked platform applications require a platform administrator.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_principal_provision_request_dto = OpenapiClient::ApplicationPrincipalProvisionRequestDto.new({business_application_id: 'business_application_id_example'}) # ApplicationPrincipalProvisionRequestDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Provision an application principal
  result = api_instance.provision_application_principal_async(tenant_id, application_principal_provision_request_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->provision_application_principal_async: #{e}"
end
```

#### Using the provision_application_principal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalProvisioningResultDtoEnvelope>, Integer, Hash)> provision_application_principal_async_with_http_info(tenant_id, application_principal_provision_request_dto, opts)

```ruby
begin
  # Provision an application principal
  data, status_code, headers = api_instance.provision_application_principal_async_with_http_info(tenant_id, application_principal_provision_request_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalProvisioningResultDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->provision_application_principal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **application_principal_provision_request_dto** | [**ApplicationPrincipalProvisionRequestDto**](ApplicationPrincipalProvisionRequestDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ApplicationPrincipalProvisioningResultDtoEnvelope**](ApplicationPrincipalProvisioningResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## revoke_permission_async

> <EmptyEnvelope> revoke_permission_async(tenant_id, principal_id, permission, opts)

Revoke a permission from an application principal

Revokes a direct permission grant from the application principal's enrollment. System-locked principals require a platform administrator.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
permission = 'permission_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a permission from an application principal
  result = api_instance.revoke_permission_async(tenant_id, principal_id, permission, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->revoke_permission_async: #{e}"
end
```

#### Using the revoke_permission_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_permission_async_with_http_info(tenant_id, principal_id, permission, opts)

```ruby
begin
  # Revoke a permission from an application principal
  data, status_code, headers = api_instance.revoke_permission_async_with_http_info(tenant_id, principal_id, permission, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->revoke_permission_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **principal_id** | **String** |  |  |
| **permission** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## suspend_application_principal_async

> <EmptyEnvelope> suspend_application_principal_async(tenant_id, principal_id, opts)

Suspend an application principal

Temporarily suspends the application principal; its identity is retained but it cannot act until reinstated.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Suspend an application principal
  result = api_instance.suspend_application_principal_async(tenant_id, principal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->suspend_application_principal_async: #{e}"
end
```

#### Using the suspend_application_principal_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> suspend_application_principal_async_with_http_info(tenant_id, principal_id, opts)

```ruby
begin
  # Suspend an application principal
  data, status_code, headers = api_instance.suspend_application_principal_async_with_http_info(tenant_id, principal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->suspend_application_principal_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **principal_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

