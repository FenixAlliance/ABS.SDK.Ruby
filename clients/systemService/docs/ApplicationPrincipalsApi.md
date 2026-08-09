# OpenapiClient::ApplicationPrincipalsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**disable_global_application_principal**](ApplicationPrincipalsApi.md#disable_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Disable | Disable an application principal (global) |
| [**enable_global_application_principal**](ApplicationPrincipalsApi.md#enable_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Enable | Enable an application principal (global) |
| [**get_global_application_principal**](ApplicationPrincipalsApi.md#get_global_application_principal) | **GET** /api/v2/SystemService/ApplicationPrincipals/{principalId} | Get one application principal (any tenant) |
| [**get_global_application_principals**](ApplicationPrincipalsApi.md#get_global_application_principals) | **GET** /api/v2/SystemService/ApplicationPrincipals | List application principals across all tenants |
| [**get_global_application_principals_count**](ApplicationPrincipalsApi.md#get_global_application_principals_count) | **GET** /api/v2/SystemService/ApplicationPrincipals/Count | Count application principals across all tenants |
| [**grant_global_application_principal_permission**](ApplicationPrincipalsApi.md#grant_global_application_principal_permission) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Permissions | Grant a permission to an application principal (any tenant) |
| [**provision_global_application_principal**](ApplicationPrincipalsApi.md#provision_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/Provision | Provision an application principal (any tenant, incl. system-locked) |
| [**provision_payments_connector**](ApplicationPrincipalsApi.md#provision_payments_connector) | **POST** /api/v2/SystemService/ApplicationPrincipals/PaymentsConnector | Provision the platform payments-connector identity |
| [**revoke_global_application_principal_permission**](ApplicationPrincipalsApi.md#revoke_global_application_principal_permission) | **DELETE** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Permissions/{permission} | Revoke a permission from an application principal (any tenant) |
| [**suspend_global_application_principal**](ApplicationPrincipalsApi.md#suspend_global_application_principal) | **POST** /api/v2/SystemService/ApplicationPrincipals/{principalId}/Suspend | Suspend an application principal (global) |


## disable_global_application_principal

> <EmptyEnvelope> disable_global_application_principal(principal_id, tenant_id, opts)

Disable an application principal (global)

Disables the application principal; dependent unattended execution fails closed (applies to system-locked principals here). tenantId scopes the action to a tenant the principal is enrolled in (required). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Disable an application principal (global)
  result = api_instance.disable_global_application_principal(principal_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->disable_global_application_principal: #{e}"
end
```

#### Using the disable_global_application_principal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> disable_global_application_principal_with_http_info(principal_id, tenant_id, opts)

```ruby
begin
  # Disable an application principal (global)
  data, status_code, headers = api_instance.disable_global_application_principal_with_http_info(principal_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->disable_global_application_principal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principal_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## enable_global_application_principal

> <EmptyEnvelope> enable_global_application_principal(principal_id, tenant_id, opts)

Enable an application principal (global)

Reinstates the application principal to the Active lifecycle state (applies to system-locked principals here). tenantId scopes the action to a tenant the principal is enrolled in (required). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Enable an application principal (global)
  result = api_instance.enable_global_application_principal(principal_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->enable_global_application_principal: #{e}"
end
```

#### Using the enable_global_application_principal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> enable_global_application_principal_with_http_info(principal_id, tenant_id, opts)

```ruby
begin
  # Enable an application principal (global)
  data, status_code, headers = api_instance.enable_global_application_principal_with_http_info(principal_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->enable_global_application_principal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principal_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_global_application_principal

> <ApplicationPrincipalDetailDtoEnvelope> get_global_application_principal(principal_id, opts)

Get one application principal (any tenant)

Returns one application principal's detail by id: owning application, an enrollment, the system-locked flag, lifecycle status, and that enrollment's explicit least-privilege grants. Pass tenantId to select the enrollment for a multi-tenant principal; when omitted the principal's first enrollment is used. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get one application principal (any tenant)
  result = api_instance.get_global_application_principal(principal_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_global_application_principal: #{e}"
end
```

#### Using the get_global_application_principal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalDetailDtoEnvelope>, Integer, Hash)> get_global_application_principal_with_http_info(principal_id, opts)

```ruby
begin
  # Get one application principal (any tenant)
  data, status_code, headers = api_instance.get_global_application_principal_with_http_info(principal_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalDetailDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_global_application_principal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principal_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ApplicationPrincipalDetailDtoEnvelope**](ApplicationPrincipalDetailDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_global_application_principals

> <ApplicationPrincipalDtoIReadOnlyListEnvelope> get_global_application_principals(opts)

List application principals across all tenants

Lists every non-human application principal enrollment across ALL tenants (payload-safe fields only), including the platform-managed (system-locked) connectors. Use OData to scope — e.g. $filter=SystemLocked eq true for the platform connectors or TenantId eq '{guid}' for one tenant — and to page/order. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  application_principal_dto_collection_query_parameters: OpenapiClient::ApplicationPrincipalDtoCollectionQueryParameters.new # ApplicationPrincipalDtoCollectionQueryParameters | 
}

begin
  # List application principals across all tenants
  result = api_instance.get_global_application_principals(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_global_application_principals: #{e}"
end
```

#### Using the get_global_application_principals_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalDtoIReadOnlyListEnvelope>, Integer, Hash)> get_global_application_principals_with_http_info(opts)

```ruby
begin
  # List application principals across all tenants
  data, status_code, headers = api_instance.get_global_application_principals_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalDtoIReadOnlyListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_global_application_principals_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **application_principal_dto_collection_query_parameters** | [**ApplicationPrincipalDtoCollectionQueryParameters**](ApplicationPrincipalDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ApplicationPrincipalDtoIReadOnlyListEnvelope**](ApplicationPrincipalDtoIReadOnlyListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_global_application_principals_count

> <Int32Envelope> get_global_application_principals_count(opts)

Count application principals across all tenants

Returns the count of application principal enrollments across ALL tenants under the same OData shaping as the list read (e.g. $filter=SystemLocked eq true). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  application_principal_dto_collection_query_parameters: OpenapiClient::ApplicationPrincipalDtoCollectionQueryParameters.new # ApplicationPrincipalDtoCollectionQueryParameters | 
}

begin
  # Count application principals across all tenants
  result = api_instance.get_global_application_principals_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_global_application_principals_count: #{e}"
end
```

#### Using the get_global_application_principals_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_global_application_principals_count_with_http_info(opts)

```ruby
begin
  # Count application principals across all tenants
  data, status_code, headers = api_instance.get_global_application_principals_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->get_global_application_principals_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## grant_global_application_principal_permission

> <EmptyEnvelope> grant_global_application_principal_permission(principal_id, tenant_id, application_principal_permission_request_dto, opts)

Grant a permission to an application principal (any tenant)

Grants a single least-privilege permission to the application principal's enrollment in the tenantId tenant (grants are per-tenant, so tenantId is required). Owner/admin/wildcard/*_manage permissions are rejected even for a global admin (least-privilege by construction). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
application_principal_permission_request_dto = OpenapiClient::ApplicationPrincipalPermissionRequestDto.new({permission: 'permission_example'}) # ApplicationPrincipalPermissionRequestDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Grant a permission to an application principal (any tenant)
  result = api_instance.grant_global_application_principal_permission(principal_id, tenant_id, application_principal_permission_request_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->grant_global_application_principal_permission: #{e}"
end
```

#### Using the grant_global_application_principal_permission_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> grant_global_application_principal_permission_with_http_info(principal_id, tenant_id, application_principal_permission_request_dto, opts)

```ruby
begin
  # Grant a permission to an application principal (any tenant)
  data, status_code, headers = api_instance.grant_global_application_principal_permission_with_http_info(principal_id, tenant_id, application_principal_permission_request_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->grant_global_application_principal_permission_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principal_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
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


## provision_global_application_principal

> <ApplicationPrincipalProvisioningResultDtoEnvelope> provision_global_application_principal(application_principal_provision_request_dto, opts)

Provision an application principal (any tenant, incl. system-locked)

Idempotently provisions the application principal (and its own least-privilege enrollment) for a governed business application. tenantId selects the target tenant (defaults to the platform/root tenant). Unlike the per-tenant lane, a system-locked platform application is provisionable here. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
application_principal_provision_request_dto = OpenapiClient::ApplicationPrincipalProvisionRequestDto.new({business_application_id: 'business_application_id_example'}) # ApplicationPrincipalProvisionRequestDto | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Provision an application principal (any tenant, incl. system-locked)
  result = api_instance.provision_global_application_principal(application_principal_provision_request_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->provision_global_application_principal: #{e}"
end
```

#### Using the provision_global_application_principal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalProvisioningResultDtoEnvelope>, Integer, Hash)> provision_global_application_principal_with_http_info(application_principal_provision_request_dto, opts)

```ruby
begin
  # Provision an application principal (any tenant, incl. system-locked)
  data, status_code, headers = api_instance.provision_global_application_principal_with_http_info(application_principal_provision_request_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalProvisioningResultDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->provision_global_application_principal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **application_principal_provision_request_dto** | [**ApplicationPrincipalProvisionRequestDto**](ApplicationPrincipalProvisionRequestDto.md) |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ApplicationPrincipalProvisioningResultDtoEnvelope**](ApplicationPrincipalProvisioningResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## provision_payments_connector

> <ApplicationPrincipalProvisioningResultDtoEnvelope> provision_payments_connector(opts)

Provision the platform payments-connector identity

Idempotently stands up the platform payments-connector identity — its well-known business application, its application principal, and its own least-privilege enrollment (payments_create/payments_update/journals_post). tenantId selects the target tenant (defaults to the platform/root tenant). The provisioned connector then appears in this global list and (for its tenant) the per-tenant list. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Provision the platform payments-connector identity
  result = api_instance.provision_payments_connector(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->provision_payments_connector: #{e}"
end
```

#### Using the provision_payments_connector_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApplicationPrincipalProvisioningResultDtoEnvelope>, Integer, Hash)> provision_payments_connector_with_http_info(opts)

```ruby
begin
  # Provision the platform payments-connector identity
  data, status_code, headers = api_instance.provision_payments_connector_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApplicationPrincipalProvisioningResultDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->provision_payments_connector_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ApplicationPrincipalProvisioningResultDtoEnvelope**](ApplicationPrincipalProvisioningResultDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## revoke_global_application_principal_permission

> <EmptyEnvelope> revoke_global_application_principal_permission(principal_id, permission, tenant_id, opts)

Revoke a permission from an application principal (any tenant)

Revokes a direct permission grant from the application principal's enrollment in the tenantId tenant (required). Idempotent. Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
permission = 'permission_example' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a permission from an application principal (any tenant)
  result = api_instance.revoke_global_application_principal_permission(principal_id, permission, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->revoke_global_application_principal_permission: #{e}"
end
```

#### Using the revoke_global_application_principal_permission_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> revoke_global_application_principal_permission_with_http_info(principal_id, permission, tenant_id, opts)

```ruby
begin
  # Revoke a permission from an application principal (any tenant)
  data, status_code, headers = api_instance.revoke_global_application_principal_permission_with_http_info(principal_id, permission, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->revoke_global_application_principal_permission_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principal_id** | **String** |  |  |
| **permission** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## suspend_global_application_principal

> <EmptyEnvelope> suspend_global_application_principal(principal_id, tenant_id, opts)

Suspend an application principal (global)

Temporarily suspends the application principal; its identity is retained but it cannot act until reinstated (applies to system-locked principals here). tenantId scopes the action to a tenant the principal is enrolled in (required). Global-administrator only.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ApplicationPrincipalsApi.new
principal_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Suspend an application principal (global)
  result = api_instance.suspend_global_application_principal(principal_id, tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->suspend_global_application_principal: #{e}"
end
```

#### Using the suspend_global_application_principal_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> suspend_global_application_principal_with_http_info(principal_id, tenant_id, opts)

```ruby
begin
  # Suspend an application principal (global)
  data, status_code, headers = api_instance.suspend_global_application_principal_with_http_info(principal_id, tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ApplicationPrincipalsApi->suspend_global_application_principal_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **principal_id** | **String** |  |  |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

