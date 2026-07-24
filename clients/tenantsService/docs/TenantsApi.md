# OpenapiClient::TenantsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**assign_license_async**](TenantsApi.md#assign_license_async) | **POST** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses/{licenseId} | Assign a license to a specific enrollment |
| [**create_tenant_async**](TenantsApi.md#create_tenant_async) | **POST** /api/v2/TenantsService/Tenants | Create a new business tenant |
| [**de_select_tenant_async**](TenantsApi.md#de_select_tenant_async) | **POST** /api/v2/TenantsService/Tenants/Deselect | Deselect the user&#39;s default tenant |
| [**delete_tenant_async**](TenantsApi.md#delete_tenant_async) | **DELETE** /api/v2/TenantsService/Tenants | Delete a tenant |
| [**get_accessible_features_async**](TenantsApi.md#get_accessible_features_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Features | Get the list of features accessible to a specific enrollment |
| [**get_cart_for_tenant_async**](TenantsApi.md#get_cart_for_tenant_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Cart | Get a tenant&#39;s default cart |
| [**get_current_tenant_async**](TenantsApi.md#get_current_tenant_async) | **GET** /api/v2/TenantsService/Tenants/Current | Get the user&#39;s current default tenant |
| [**get_enrollment_license_by_id_async**](TenantsApi.md#get_enrollment_license_by_id_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses/{licenseId} | Get a specific license for an enrollment |
| [**get_enrollment_licenses_async**](TenantsApi.md#get_enrollment_licenses_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses | Get the list of licenses available to a specific enrollment |
| [**get_enrollment_permissions_async**](TenantsApi.md#get_enrollment_permissions_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Permissions | Get a specific tenant enrollment&#39;s permissions list |
| [**get_extended_tenant_async**](TenantsApi.md#get_extended_tenant_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Extended | Get an extended tenant&#39;s business profile |
| [**get_extended_tenant_enrollment_async**](TenantsApi.md#get_extended_tenant_enrollment_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Extended | Get a specific tenant enrollment |
| [**get_root_tenant_async**](TenantsApi.md#get_root_tenant_async) | **GET** /api/v2/TenantsService/Tenants/Root | Get the root tenant of the platform |
| [**get_tenant_async**](TenantsApi.md#get_tenant_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId} | Get a specific tenant by ID |
| [**get_tenant_avatar_async**](TenantsApi.md#get_tenant_avatar_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Avatar | Get a tenant&#39;s avatar |
| [**get_tenant_enrollment_async**](TenantsApi.md#get_tenant_enrollment_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId} | Get a specific tenant enrollment |
| [**get_tenant_enrollments_async**](TenantsApi.md#get_tenant_enrollments_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments | Get the list of user enrollments for a tenant |
| [**get_tenant_invitations_async**](TenantsApi.md#get_tenant_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations | Get the list of invitations issued by a tenant |
| [**get_tenant_licenses_async**](TenantsApi.md#get_tenant_licenses_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Licenses | Get the list of licenses available to a tenant |
| [**get_tenant_notifications_async**](TenantsApi.md#get_tenant_notifications_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Notifications | Get the list of notifications for a tenant |
| [**get_tenant_notifications_count_async**](TenantsApi.md#get_tenant_notifications_count_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Notifications/Count | Get the count of notifications for a tenant |
| [**get_tenant_pending_invitations_async**](TenantsApi.md#get_tenant_pending_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations/Pending | Get the list of invitations issued by a tenant that are pending |
| [**get_tenant_redeemed_invitations_async**](TenantsApi.md#get_tenant_redeemed_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations/Redeemed | Get the list of invitations issued by a tenant that have been redeemed |
| [**get_tenant_revoked_invitations_async**](TenantsApi.md#get_tenant_revoked_invitations_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Invitations/Revoked | Get the list of invitations issued by a tenant that have been revoked |
| [**get_tenant_social_profile_async**](TenantsApi.md#get_tenant_social_profile_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/SocialProfile | Get a tenant&#39;s social profile |
| [**get_tenant_users_async**](TenantsApi.md#get_tenant_users_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Users | Get the list of users enrolled in a tenant |
| [**get_tenant_wallet_async**](TenantsApi.md#get_tenant_wallet_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Wallet | Get a tenant&#39;s billing profile (A.K.A. Wallet Account) |
| [**get_tenant_web_portals_async**](TenantsApi.md#get_tenant_web_portals_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/WebPortals | Get the list of web portals for a tenant |
| [**patch_tenant_async**](TenantsApi.md#patch_tenant_async) | **PATCH** /api/v2/TenantsService/Tenants/{tenantId} | Patch a tenant&#39;s profile |
| [**revoke_license_async**](TenantsApi.md#revoke_license_async) | **DELETE** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Licenses/{licenseId} | Revoke a license from a specific enrollment |
| [**select_tenant_async**](TenantsApi.md#select_tenant_async) | **POST** /api/v2/TenantsService/Tenants/{tenantId}/Select | Select a business tenant as the user&#39;s default tenant |
| [**update_tenant_async**](TenantsApi.md#update_tenant_async) | **PUT** /api/v2/TenantsService/Tenants/{tenantId} | Update a tenant&#39;s profile |
| [**update_tenant_avatar_async**](TenantsApi.md#update_tenant_avatar_async) | **POST** /api/v2/TenantsService/Tenants/{tenantId}/Avatar | Update a tenant&#39;s avatar |
| [**validate_enrollment_feature_access**](TenantsApi.md#validate_enrollment_feature_access) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/HasAccess | Validate the access to a specific feature for a specific enrollment |
| [**validate_enrollment_permissions_async**](TenantsApi.md#validate_enrollment_permissions_async) | **GET** /api/v2/TenantsService/Tenants/{tenantId}/Enrollments/{enrollmentId}/Permissions/Validate | Validate the existence of a list of roles and permissions for a specific enrollment |


## assign_license_async

> <SuiteLicenseDtoListEnvelope> assign_license_async(tenant_id, enrollment_id, license_id, opts)

Assign a license to a specific enrollment

Assign a license to a specific enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
license_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Assign a license to a specific enrollment
  result = api_instance.assign_license_async(tenant_id, enrollment_id, license_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->assign_license_async: #{e}"
end
```

#### Using the assign_license_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SuiteLicenseDtoListEnvelope>, Integer, Hash)> assign_license_async_with_http_info(tenant_id, enrollment_id, license_id, opts)

```ruby
begin
  # Assign a license to a specific enrollment
  data, status_code, headers = api_instance.assign_license_async_with_http_info(tenant_id, enrollment_id, license_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SuiteLicenseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->assign_license_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **license_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_tenant_async

> <EmptyEnvelope> create_tenant_async(opts)

Create a new business tenant

Create a new business tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_create_dto: OpenapiClient::TenantCreateDto.new({name: 'name_example', email: 'email_example', currency_id: 'currency_id_example', country_id: 'country_id_example'}) # TenantCreateDto | 
}

begin
  # Create a new business tenant
  result = api_instance.create_tenant_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->create_tenant_async: #{e}"
end
```

#### Using the create_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_async_with_http_info(opts)

```ruby
begin
  # Create a new business tenant
  data, status_code, headers = api_instance.create_tenant_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->create_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_create_dto** | [**TenantCreateDto**](TenantCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## de_select_tenant_async

> <EmptyEnvelope> de_select_tenant_async(opts)

Deselect the user's default tenant

Deselect the user's default tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Deselect the user's default tenant
  result = api_instance.de_select_tenant_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->de_select_tenant_async: #{e}"
end
```

#### Using the de_select_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> de_select_tenant_async_with_http_info(opts)

```ruby
begin
  # Deselect the user's default tenant
  data, status_code, headers = api_instance.de_select_tenant_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->de_select_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_tenant_async

> <EmptyEnvelope> delete_tenant_async(tenant_id, opts)

Delete a tenant

Delete a business tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant
  result = api_instance.delete_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->delete_tenant_async: #{e}"
end
```

#### Using the delete_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Delete a tenant
  data, status_code, headers = api_instance.delete_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->delete_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_accessible_features_async

> <SuiteLicenseFeatureDtoListEnvelope> get_accessible_features_async(tenant_id, enrollment_id, opts)

Get the list of features accessible to a specific enrollment

Get the list of features accessible to a specific enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of features accessible to a specific enrollment
  result = api_instance.get_accessible_features_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_accessible_features_async: #{e}"
end
```

#### Using the get_accessible_features_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SuiteLicenseFeatureDtoListEnvelope>, Integer, Hash)> get_accessible_features_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get the list of features accessible to a specific enrollment
  data, status_code, headers = api_instance.get_accessible_features_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SuiteLicenseFeatureDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_accessible_features_async_with_http_info: #{e}"
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

[**SuiteLicenseFeatureDtoListEnvelope**](SuiteLicenseFeatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_cart_for_tenant_async

> <CartDtoEnvelope> get_cart_for_tenant_async(tenant_id, opts)

Get a tenant's default cart

Get a tenant's default cart

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a tenant's default cart
  result = api_instance.get_cart_for_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_cart_for_tenant_async: #{e}"
end
```

#### Using the get_cart_for_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CartDtoEnvelope>, Integer, Hash)> get_cart_for_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get a tenant's default cart
  data, status_code, headers = api_instance.get_cart_for_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CartDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_cart_for_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CartDtoEnvelope**](CartDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_current_tenant_async

> <TenantDtoEnvelope> get_current_tenant_async(tenant_id, opts)

Get the user's current default tenant

Get the user's current default tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the user's current default tenant
  result = api_instance.get_current_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_current_tenant_async: #{e}"
end
```

#### Using the get_current_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoEnvelope>, Integer, Hash)> get_current_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the user's current default tenant
  data, status_code, headers = api_instance.get_current_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_current_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollment_license_by_id_async

> <SuiteLicenseDtoListEnvelope> get_enrollment_license_by_id_async(tenant_id, enrollment_id, license_id, opts)

Get a specific license for an enrollment

Get a specific license for an enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
license_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a specific license for an enrollment
  result = api_instance.get_enrollment_license_by_id_async(tenant_id, enrollment_id, license_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_enrollment_license_by_id_async: #{e}"
end
```

#### Using the get_enrollment_license_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SuiteLicenseDtoListEnvelope>, Integer, Hash)> get_enrollment_license_by_id_async_with_http_info(tenant_id, enrollment_id, license_id, opts)

```ruby
begin
  # Get a specific license for an enrollment
  data, status_code, headers = api_instance.get_enrollment_license_by_id_async_with_http_info(tenant_id, enrollment_id, license_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SuiteLicenseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_enrollment_license_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **license_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollment_licenses_async

> <SuiteLicenseAssignmentDtoListEnvelope> get_enrollment_licenses_async(tenant_id, enrollment_id, opts)

Get the list of licenses available to a specific enrollment

Get the list of licenses available to a specific enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of licenses available to a specific enrollment
  result = api_instance.get_enrollment_licenses_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_enrollment_licenses_async: #{e}"
end
```

#### Using the get_enrollment_licenses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SuiteLicenseAssignmentDtoListEnvelope>, Integer, Hash)> get_enrollment_licenses_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get the list of licenses available to a specific enrollment
  data, status_code, headers = api_instance.get_enrollment_licenses_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SuiteLicenseAssignmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_enrollment_licenses_async_with_http_info: #{e}"
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

[**SuiteLicenseAssignmentDtoListEnvelope**](SuiteLicenseAssignmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enrollment_permissions_async

> <StringListEnvelope> get_enrollment_permissions_async(tenant_id, enrollment_id, opts)

Get a specific tenant enrollment's permissions list

Get a specific tenant enrollment's permissions list

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a specific tenant enrollment's permissions list
  result = api_instance.get_enrollment_permissions_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_enrollment_permissions_async: #{e}"
end
```

#### Using the get_enrollment_permissions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StringListEnvelope>, Integer, Hash)> get_enrollment_permissions_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get a specific tenant enrollment's permissions list
  data, status_code, headers = api_instance.get_enrollment_permissions_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StringListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_enrollment_permissions_async_with_http_info: #{e}"
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

[**StringListEnvelope**](StringListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_tenant_async

> <ExtendedTenantDtoEnvelope> get_extended_tenant_async(tenant_id, opts)

Get an extended tenant's business profile

Get an extended tenant's business profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an extended tenant's business profile
  result = api_instance.get_extended_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_extended_tenant_async: #{e}"
end
```

#### Using the get_extended_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedTenantDtoEnvelope>, Integer, Hash)> get_extended_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get an extended tenant's business profile
  data, status_code, headers = api_instance.get_extended_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedTenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_extended_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedTenantDtoEnvelope**](ExtendedTenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_tenant_enrollment_async

> <ExtendedTenantEnrollmentDtoEnvelope> get_extended_tenant_enrollment_async(tenant_id, enrollment_id, opts)

Get a specific tenant enrollment

Get a specific tenant enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a specific tenant enrollment
  result = api_instance.get_extended_tenant_enrollment_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_extended_tenant_enrollment_async: #{e}"
end
```

#### Using the get_extended_tenant_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedTenantEnrollmentDtoEnvelope>, Integer, Hash)> get_extended_tenant_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get a specific tenant enrollment
  data, status_code, headers = api_instance.get_extended_tenant_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedTenantEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_extended_tenant_enrollment_async_with_http_info: #{e}"
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

[**ExtendedTenantEnrollmentDtoEnvelope**](ExtendedTenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_root_tenant_async

> <TenantDtoEnvelope> get_root_tenant_async(opts)

Get the root tenant of the platform

Get the root tenant of the platform

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the root tenant of the platform
  result = api_instance.get_root_tenant_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_root_tenant_async: #{e}"
end
```

#### Using the get_root_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoEnvelope>, Integer, Hash)> get_root_tenant_async_with_http_info(opts)

```ruby
begin
  # Get the root tenant of the platform
  data, status_code, headers = api_instance.get_root_tenant_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_root_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_async

> <TenantDtoEnvelope> get_tenant_async(tenant_id, opts)

Get a specific tenant by ID

Get a specific tenant by ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a specific tenant by ID
  result = api_instance.get_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_async: #{e}"
end
```

#### Using the get_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoEnvelope>, Integer, Hash)> get_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get a specific tenant by ID
  data, status_code, headers = api_instance.get_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_avatar_async

> <EmptyEnvelope> get_tenant_avatar_async(tenant_id, opts)

Get a tenant's avatar

Get a tenant's avatar

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a tenant's avatar
  result = api_instance.get_tenant_avatar_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_avatar_async: #{e}"
end
```

#### Using the get_tenant_avatar_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> get_tenant_avatar_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get a tenant's avatar
  data, status_code, headers = api_instance.get_tenant_avatar_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_avatar_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## get_tenant_enrollment_async

> <TenantEnrollmentDtoEnvelope> get_tenant_enrollment_async(tenant_id, enrollment_id, opts)

Get a specific tenant enrollment

Get a specific tenant enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a specific tenant enrollment
  result = api_instance.get_tenant_enrollment_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_enrollment_async: #{e}"
end
```

#### Using the get_tenant_enrollment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoEnvelope>, Integer, Hash)> get_tenant_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Get a specific tenant enrollment
  data, status_code, headers = api_instance.get_tenant_enrollment_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_enrollment_async_with_http_info: #{e}"
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

[**TenantEnrollmentDtoEnvelope**](TenantEnrollmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_enrollments_async

> <TenantEnrollmentDtoListEnvelope> get_tenant_enrollments_async(tenant_id, opts)

Get the list of user enrollments for a tenant

Get the list of user enrollments for a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of user enrollments for a tenant
  result = api_instance.get_tenant_enrollments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_enrollments_async: #{e}"
end
```

#### Using the get_tenant_enrollments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantEnrollmentDtoListEnvelope>, Integer, Hash)> get_tenant_enrollments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of user enrollments for a tenant
  data, status_code, headers = api_instance.get_tenant_enrollments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantEnrollmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_enrollments_async_with_http_info: #{e}"
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


## get_tenant_invitations_async

> <TenantInvitationDtoListEnvelope> get_tenant_invitations_async(tenant_id, opts)

Get the list of invitations issued by a tenant

Get the list of invitations issued by a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of invitations issued by a tenant
  result = api_instance.get_tenant_invitations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_invitations_async: #{e}"
end
```

#### Using the get_tenant_invitations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoListEnvelope>, Integer, Hash)> get_tenant_invitations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of invitations issued by a tenant
  data, status_code, headers = api_instance.get_tenant_invitations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_invitations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_licenses_async

> <SuiteLicenseDtoListEnvelope> get_tenant_licenses_async(tenant_id, opts)

Get the list of licenses available to a tenant

Get the list of licenses available to a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of licenses available to a tenant
  result = api_instance.get_tenant_licenses_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_licenses_async: #{e}"
end
```

#### Using the get_tenant_licenses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SuiteLicenseDtoListEnvelope>, Integer, Hash)> get_tenant_licenses_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of licenses available to a tenant
  data, status_code, headers = api_instance.get_tenant_licenses_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SuiteLicenseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_licenses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_notifications_async

> <NotificationDtoListEnvelope> get_tenant_notifications_async(tenant_id, opts)

Get the list of notifications for a tenant

Get the list of notifications for a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of notifications for a tenant
  result = api_instance.get_tenant_notifications_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_notifications_async: #{e}"
end
```

#### Using the get_tenant_notifications_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NotificationDtoListEnvelope>, Integer, Hash)> get_tenant_notifications_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of notifications for a tenant
  data, status_code, headers = api_instance.get_tenant_notifications_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NotificationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_notifications_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**NotificationDtoListEnvelope**](NotificationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_notifications_count_async

> <Int32Envelope> get_tenant_notifications_count_async(tenant_id, opts)

Get the count of notifications for a tenant

Get the count of notifications for a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of notifications for a tenant
  result = api_instance.get_tenant_notifications_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_notifications_count_async: #{e}"
end
```

#### Using the get_tenant_notifications_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_notifications_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of notifications for a tenant
  data, status_code, headers = api_instance.get_tenant_notifications_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_notifications_count_async_with_http_info: #{e}"
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


## get_tenant_pending_invitations_async

> <TenantInvitationDtoListEnvelope> get_tenant_pending_invitations_async(tenant_id, opts)

Get the list of invitations issued by a tenant that are pending

Get the list of invitations issued by a tenant that are pending

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of invitations issued by a tenant that are pending
  result = api_instance.get_tenant_pending_invitations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_pending_invitations_async: #{e}"
end
```

#### Using the get_tenant_pending_invitations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoListEnvelope>, Integer, Hash)> get_tenant_pending_invitations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of invitations issued by a tenant that are pending
  data, status_code, headers = api_instance.get_tenant_pending_invitations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_pending_invitations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_redeemed_invitations_async

> <TenantInvitationDtoListEnvelope> get_tenant_redeemed_invitations_async(tenant_id, opts)

Get the list of invitations issued by a tenant that have been redeemed

Get the list of invitations issued by a tenant that have been redeemed

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of invitations issued by a tenant that have been redeemed
  result = api_instance.get_tenant_redeemed_invitations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_redeemed_invitations_async: #{e}"
end
```

#### Using the get_tenant_redeemed_invitations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoListEnvelope>, Integer, Hash)> get_tenant_redeemed_invitations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of invitations issued by a tenant that have been redeemed
  data, status_code, headers = api_instance.get_tenant_redeemed_invitations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_redeemed_invitations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_revoked_invitations_async

> <TenantInvitationDtoListEnvelope> get_tenant_revoked_invitations_async(tenant_id, opts)

Get the list of invitations issued by a tenant that have been revoked

Get the list of invitations issued by a tenant that have been revoked

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of invitations issued by a tenant that have been revoked
  result = api_instance.get_tenant_revoked_invitations_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_revoked_invitations_async: #{e}"
end
```

#### Using the get_tenant_revoked_invitations_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantInvitationDtoListEnvelope>, Integer, Hash)> get_tenant_revoked_invitations_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of invitations issued by a tenant that have been revoked
  data, status_code, headers = api_instance.get_tenant_revoked_invitations_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantInvitationDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_revoked_invitations_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantInvitationDtoListEnvelope**](TenantInvitationDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_social_profile_async

> <SocialProfileDtoEnvelope> get_tenant_social_profile_async(tenant_id, opts)

Get a tenant's social profile

Get a tenant's social profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a tenant's social profile
  result = api_instance.get_tenant_social_profile_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_social_profile_async: #{e}"
end
```

#### Using the get_tenant_social_profile_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SocialProfileDtoEnvelope>, Integer, Hash)> get_tenant_social_profile_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get a tenant's social profile
  data, status_code, headers = api_instance.get_tenant_social_profile_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SocialProfileDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_social_profile_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SocialProfileDtoEnvelope**](SocialProfileDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_users_async

> <UserDtoListEnvelope> get_tenant_users_async(tenant_id, opts)

Get the list of users enrolled in a tenant

Get the list of users enrolled in a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of users enrolled in a tenant
  result = api_instance.get_tenant_users_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_users_async: #{e}"
end
```

#### Using the get_tenant_users_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserDtoListEnvelope>, Integer, Hash)> get_tenant_users_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of users enrolled in a tenant
  data, status_code, headers = api_instance.get_tenant_users_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_users_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**UserDtoListEnvelope**](UserDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_wallet_async

> <WalletDtoEnvelope> get_tenant_wallet_async(tenant_id, opts)

Get a tenant's billing profile (A.K.A. Wallet Account)

Get a tenant's billing profile (A.K.A. Wallet Account)

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a tenant's billing profile (A.K.A. Wallet Account)
  result = api_instance.get_tenant_wallet_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_wallet_async: #{e}"
end
```

#### Using the get_tenant_wallet_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WalletDtoEnvelope>, Integer, Hash)> get_tenant_wallet_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get a tenant's billing profile (A.K.A. Wallet Account)
  data, status_code, headers = api_instance.get_tenant_wallet_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WalletDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_wallet_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WalletDtoEnvelope**](WalletDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_web_portals_async

> <WebPortalDtoListEnvelope> get_tenant_web_portals_async(tenant_id, opts)

Get the list of web portals for a tenant

Get the list of web portals for a tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the list of web portals for a tenant
  result = api_instance.get_tenant_web_portals_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_web_portals_async: #{e}"
end
```

#### Using the get_tenant_web_portals_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebPortalDtoListEnvelope>, Integer, Hash)> get_tenant_web_portals_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the list of web portals for a tenant
  data, status_code, headers = api_instance.get_tenant_web_portals_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebPortalDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_web_portals_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebPortalDtoListEnvelope**](WebPortalDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_tenant_async

> <EmptyEnvelope> patch_tenant_async(tenant_id, opts)

Patch a tenant's profile

Patch a tenant's profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a tenant's profile
  result = api_instance.patch_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->patch_tenant_async: #{e}"
end
```

#### Using the patch_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Patch a tenant's profile
  data, status_code, headers = api_instance.patch_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->patch_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
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


## revoke_license_async

> <SuiteLicenseDtoListEnvelope> revoke_license_async(tenant_id, enrollment_id, license_id, opts)

Revoke a license from a specific enrollment

Revoke a license from a specific enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
license_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Revoke a license from a specific enrollment
  result = api_instance.revoke_license_async(tenant_id, enrollment_id, license_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->revoke_license_async: #{e}"
end
```

#### Using the revoke_license_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SuiteLicenseDtoListEnvelope>, Integer, Hash)> revoke_license_async_with_http_info(tenant_id, enrollment_id, license_id, opts)

```ruby
begin
  # Revoke a license from a specific enrollment
  data, status_code, headers = api_instance.revoke_license_async_with_http_info(tenant_id, enrollment_id, license_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SuiteLicenseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->revoke_license_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **license_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SuiteLicenseDtoListEnvelope**](SuiteLicenseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## select_tenant_async

> <EmptyEnvelope> select_tenant_async(tenant_id, opts)

Select a business tenant as the user's default tenant

Select a business tenant as the user's default tenant

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Select a business tenant as the user's default tenant
  result = api_instance.select_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->select_tenant_async: #{e}"
end
```

#### Using the select_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> select_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Select a business tenant as the user's default tenant
  data, status_code, headers = api_instance.select_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->select_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
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


## update_tenant_async

> <EmptyEnvelope> update_tenant_async(tenant_id, opts)

Update a tenant's profile

Update a tenant's profile

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_update_dto: OpenapiClient::TenantUpdateDto.new({name: 'name_example', email: 'email_example', currency_id: 'currency_id_example', country_id: 'country_id_example'}) # TenantUpdateDto | 
}

begin
  # Update a tenant's profile
  result = api_instance.update_tenant_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->update_tenant_async: #{e}"
end
```

#### Using the update_tenant_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Update a tenant's profile
  data, status_code, headers = api_instance.update_tenant_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->update_tenant_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_update_dto** | [**TenantUpdateDto**](TenantUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_tenant_avatar_async

> <EmptyEnvelope> update_tenant_avatar_async(tenant_id, opts)

Update a tenant's avatar

Update a tenant's avatar

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  avatar: File.new('/path/to/some/file') # File | 
}

begin
  # Update a tenant's avatar
  result = api_instance.update_tenant_avatar_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->update_tenant_avatar_async: #{e}"
end
```

#### Using the update_tenant_avatar_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_avatar_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Update a tenant's avatar
  data, status_code, headers = api_instance.update_tenant_avatar_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->update_tenant_avatar_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **avatar** | **File** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: image/png, application/json, application/xml


## validate_enrollment_feature_access

> <BooleanEnvelope> validate_enrollment_feature_access(tenant_id, enrollment_id, opts)

Validate the access to a specific feature for a specific enrollment

Validate the access to a specific feature for a specific enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  feature: 'feature_example', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Validate the access to a specific feature for a specific enrollment
  result = api_instance.validate_enrollment_feature_access(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->validate_enrollment_feature_access: #{e}"
end
```

#### Using the validate_enrollment_feature_access_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> validate_enrollment_feature_access_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Validate the access to a specific feature for a specific enrollment
  data, status_code, headers = api_instance.validate_enrollment_feature_access_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->validate_enrollment_feature_access_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **feature** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## validate_enrollment_permissions_async

> <BooleanEnvelope> validate_enrollment_permissions_async(tenant_id, enrollment_id, opts)

Validate the existence of a list of roles and permissions for a specific enrollment

Validate the existence of a list of roles and permissions for a specific enrollment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
enrollment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  roles: ['inner_example'], # Array<String> | 
  permissions: ['inner_example'], # Array<String> | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Validate the existence of a list of roles and permissions for a specific enrollment
  result = api_instance.validate_enrollment_permissions_async(tenant_id, enrollment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->validate_enrollment_permissions_async: #{e}"
end
```

#### Using the validate_enrollment_permissions_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> validate_enrollment_permissions_async_with_http_info(tenant_id, enrollment_id, opts)

```ruby
begin
  # Validate the existence of a list of roles and permissions for a specific enrollment
  data, status_code, headers = api_instance.validate_enrollment_permissions_async_with_http_info(tenant_id, enrollment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->validate_enrollment_permissions_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **enrollment_id** | **String** |  |  |
| **roles** | [**Array&lt;String&gt;**](String.md) |  | [optional] |
| **permissions** | [**Array&lt;String&gt;**](String.md) |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

