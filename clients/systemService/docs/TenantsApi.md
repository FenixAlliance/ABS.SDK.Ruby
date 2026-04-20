# OpenapiClient::TenantsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**admin_preview_tenant_email**](TenantsApi.md#admin_preview_tenant_email) | **POST** /api/v2/SystemService/Tenants/{tenantId}/Emails/Preview | Preview the rendered email for a user. |
| [**admin_send_tenant_email**](TenantsApi.md#admin_send_tenant_email) | **POST** /api/v2/SystemService/Tenants/{tenantId}/Emails/Send | Send an email to a user. |
| [**create_tenant**](TenantsApi.md#create_tenant) | **POST** /api/v2/SystemService/Tenants | Create a new tenant. |
| [**delete_tenant**](TenantsApi.md#delete_tenant) | **DELETE** /api/v2/SystemService/Tenants/{tenantId} | Delete a specific tenant by ID. |
| [**get_all_extended_tenants**](TenantsApi.md#get_all_extended_tenants) | **GET** /api/v2/SystemService/Tenants/Extended | Get all extended tenants available on this suite server instance. |
| [**get_all_tenants**](TenantsApi.md#get_all_tenants) | **GET** /api/v2/SystemService/Tenants | Get all tenants available on this suite server instance. |
| [**get_extended_tenants_count**](TenantsApi.md#get_extended_tenants_count) | **GET** /api/v2/SystemService/Tenants/Extended/Count | Get the total count of extended tenants available on this suite server instance. |
| [**get_tenant**](TenantsApi.md#get_tenant) | **GET** /api/v2/SystemService/Tenants/{tenantId} | Get a specific tenant by ID. |
| [**get_tenants_count**](TenantsApi.md#get_tenants_count) | **GET** /api/v2/SystemService/Tenants/Count | Get the total count of tenants available on this suite server instance. |
| [**update_tenant**](TenantsApi.md#update_tenant) | **PUT** /api/v2/SystemService/Tenants/{tenantId} | Update a specific tenant by ID. |


## admin_preview_tenant_email

> admin_preview_tenant_email(tenant_id, opts)

Preview the rendered email for a user.

This action is only available for users with the 'business_owner' role (global administrators).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Preview the rendered email for a user.
  api_instance.admin_preview_tenant_email(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->admin_preview_tenant_email: #{e}"
end
```

#### Using the admin_preview_tenant_email_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> admin_preview_tenant_email_with_http_info(tenant_id, opts)

```ruby
begin
  # Preview the rendered email for a user.
  data, status_code, headers = api_instance.admin_preview_tenant_email_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->admin_preview_tenant_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## admin_send_tenant_email

> admin_send_tenant_email(tenant_id, opts)

Send an email to a user.

This action is only available for users with the 'business_owner' role (global administrators).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TenantsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  email_dispatch_request: OpenapiClient::EmailDispatchRequest.new({title: 'title_example', message: 'message_example', culture: 'culture_example', ui_culture: 'ui_culture_example', recipients: ['recipients_example']}) # EmailDispatchRequest | 
}

begin
  # Send an email to a user.
  api_instance.admin_send_tenant_email(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->admin_send_tenant_email: #{e}"
end
```

#### Using the admin_send_tenant_email_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> admin_send_tenant_email_with_http_info(tenant_id, opts)

```ruby
begin
  # Send an email to a user.
  data, status_code, headers = api_instance.admin_send_tenant_email_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->admin_send_tenant_email_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **email_dispatch_request** | [**EmailDispatchRequest**](EmailDispatchRequest.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## create_tenant

> <TenantDtoEnvelope> create_tenant(opts)

Create a new tenant.

This action is only available for global administrators.

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
  # Create a new tenant.
  result = api_instance.create_tenant(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->create_tenant: #{e}"
end
```

#### Using the create_tenant_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoEnvelope>, Integer, Hash)> create_tenant_with_http_info(opts)

```ruby
begin
  # Create a new tenant.
  data, status_code, headers = api_instance.create_tenant_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->create_tenant_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_create_dto** | [**TenantCreateDto**](TenantCreateDto.md) |  | [optional] |

### Return type

[**TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant

> <EmptyEnvelope> delete_tenant(tenant_id, opts)

Delete a specific tenant by ID.

This action is only available for global administrators.

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
  # Delete a specific tenant by ID.
  result = api_instance.delete_tenant(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->delete_tenant: #{e}"
end
```

#### Using the delete_tenant_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_with_http_info(tenant_id, opts)

```ruby
begin
  # Delete a specific tenant by ID.
  data, status_code, headers = api_instance.delete_tenant_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->delete_tenant_with_http_info: #{e}"
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


## get_all_extended_tenants

> <ExtendedTenantDtoListEnvelope> get_all_extended_tenants(opts)

Get all extended tenants available on this suite server instance.

This action is only available for global administrators.

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
  # Get all extended tenants available on this suite server instance.
  result = api_instance.get_all_extended_tenants(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_all_extended_tenants: #{e}"
end
```

#### Using the get_all_extended_tenants_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExtendedTenantDtoListEnvelope>, Integer, Hash)> get_all_extended_tenants_with_http_info(opts)

```ruby
begin
  # Get all extended tenants available on this suite server instance.
  data, status_code, headers = api_instance.get_all_extended_tenants_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExtendedTenantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_all_extended_tenants_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExtendedTenantDtoListEnvelope**](ExtendedTenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_all_tenants

> <TenantDtoListEnvelope> get_all_tenants(opts)

Get all tenants available on this suite server instance.

This action is only available for global administrators.

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
  # Get all tenants available on this suite server instance.
  result = api_instance.get_all_tenants(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_all_tenants: #{e}"
end
```

#### Using the get_all_tenants_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoListEnvelope>, Integer, Hash)> get_all_tenants_with_http_info(opts)

```ruby
begin
  # Get all tenants available on this suite server instance.
  data, status_code, headers = api_instance.get_all_tenants_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_all_tenants_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantDtoListEnvelope**](TenantDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_extended_tenants_count

> <Int32Envelope> get_extended_tenants_count(opts)

Get the total count of extended tenants available on this suite server instance.

This action is only available for global administrators.

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
  # Get the total count of extended tenants available on this suite server instance.
  result = api_instance.get_extended_tenants_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_extended_tenants_count: #{e}"
end
```

#### Using the get_extended_tenants_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_extended_tenants_count_with_http_info(opts)

```ruby
begin
  # Get the total count of extended tenants available on this suite server instance.
  data, status_code, headers = api_instance.get_extended_tenants_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_extended_tenants_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant

> <TenantDtoEnvelope> get_tenant(tenant_id, opts)

Get a specific tenant by ID.

This action is only available for global administrators.

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
  # Get a specific tenant by ID.
  result = api_instance.get_tenant(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant: #{e}"
end
```

#### Using the get_tenant_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoEnvelope>, Integer, Hash)> get_tenant_with_http_info(tenant_id, opts)

```ruby
begin
  # Get a specific tenant by ID.
  data, status_code, headers = api_instance.get_tenant_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenant_with_http_info: #{e}"
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


## get_tenants_count

> <Int32Envelope> get_tenants_count(opts)

Get the total count of tenants available on this suite server instance.

This action is only available for global administrators.

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
  # Get the total count of tenants available on this suite server instance.
  result = api_instance.get_tenants_count(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenants_count: #{e}"
end
```

#### Using the get_tenants_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenants_count_with_http_info(opts)

```ruby
begin
  # Get the total count of tenants available on this suite server instance.
  data, status_code, headers = api_instance.get_tenants_count_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->get_tenants_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_tenant

> <TenantDtoEnvelope> update_tenant(tenant_id, opts)

Update a specific tenant by ID.

This action is only available for global administrators.

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
  # Update a specific tenant by ID.
  result = api_instance.update_tenant(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->update_tenant: #{e}"
end
```

#### Using the update_tenant_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantDtoEnvelope>, Integer, Hash)> update_tenant_with_http_info(tenant_id, opts)

```ruby
begin
  # Update a specific tenant by ID.
  data, status_code, headers = api_instance.update_tenant_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TenantsApi->update_tenant_with_http_info: #{e}"
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

[**TenantDtoEnvelope**](TenantDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

