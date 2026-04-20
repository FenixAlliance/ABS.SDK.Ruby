# OpenapiClient::SyncApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**sync_current_holder_to_current_tenant_crm**](SyncApi.md#sync_current_holder_to_current_tenant_crm) | **POST** /api/v2/CrmService/Sync | Sync the current user into the current tenant&#39;s contact list |
| [**sync_current_holder_to_tenant_crm**](SyncApi.md#sync_current_holder_to_tenant_crm) | **POST** /api/v2/CrmService/Sync/Me | Sync the current user into a tenant&#39;s contact list |
| [**sync_holder_to_tenant_crm_async**](SyncApi.md#sync_holder_to_tenant_crm_async) | **POST** /api/v2/CrmService/Sync/User | Sync a user into a tenant&#39;s contact list |
| [**sync_tenant_to_tenant_crm**](SyncApi.md#sync_tenant_to_tenant_crm) | **POST** /api/v2/CrmService/Sync/Tenant | Sync a tenant into another tenant&#39;s contact list |


## sync_current_holder_to_current_tenant_crm

> <Envelope> sync_current_holder_to_current_tenant_crm(tenant_id, opts)

Sync the current user into the current tenant's contact list

Synchronizes the currently authenticated user into the current tenant's CRM contact list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SyncApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sync the current user into the current tenant's contact list
  result = api_instance.sync_current_holder_to_current_tenant_crm(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_current_holder_to_current_tenant_crm: #{e}"
end
```

#### Using the sync_current_holder_to_current_tenant_crm_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> sync_current_holder_to_current_tenant_crm_with_http_info(tenant_id, opts)

```ruby
begin
  # Sync the current user into the current tenant's contact list
  data, status_code, headers = api_instance.sync_current_holder_to_current_tenant_crm_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_current_holder_to_current_tenant_crm_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## sync_current_holder_to_tenant_crm

> <Envelope> sync_current_holder_to_tenant_crm(tenant_id, opts)

Sync the current user into a tenant's contact list

Synchronizes the currently authenticated user into the specified tenant's CRM contact list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SyncApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sync the current user into a tenant's contact list
  result = api_instance.sync_current_holder_to_tenant_crm(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_current_holder_to_tenant_crm: #{e}"
end
```

#### Using the sync_current_holder_to_tenant_crm_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> sync_current_holder_to_tenant_crm_with_http_info(tenant_id, opts)

```ruby
begin
  # Sync the current user into a tenant's contact list
  data, status_code, headers = api_instance.sync_current_holder_to_tenant_crm_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_current_holder_to_tenant_crm_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## sync_holder_to_tenant_crm_async

> <Envelope> sync_holder_to_tenant_crm_async(tenant_id, related_user_id, opts)

Sync a user into a tenant's contact list

Synchronizes a specified user into the tenant's CRM contact list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SyncApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
related_user_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sync a user into a tenant's contact list
  result = api_instance.sync_holder_to_tenant_crm_async(tenant_id, related_user_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_holder_to_tenant_crm_async: #{e}"
end
```

#### Using the sync_holder_to_tenant_crm_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Envelope>, Integer, Hash)> sync_holder_to_tenant_crm_async_with_http_info(tenant_id, related_user_id, opts)

```ruby
begin
  # Sync a user into a tenant's contact list
  data, status_code, headers = api_instance.sync_holder_to_tenant_crm_async_with_http_info(tenant_id, related_user_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_holder_to_tenant_crm_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **related_user_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Envelope**](Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## sync_tenant_to_tenant_crm

> <EmptyEnvelope> sync_tenant_to_tenant_crm(tenant_id, related_tenant_id, opts)

Sync a tenant into another tenant's contact list

Synchronizes a tenant into another tenant's CRM contact list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SyncApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
related_tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Sync a tenant into another tenant's contact list
  result = api_instance.sync_tenant_to_tenant_crm(tenant_id, related_tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_tenant_to_tenant_crm: #{e}"
end
```

#### Using the sync_tenant_to_tenant_crm_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> sync_tenant_to_tenant_crm_with_http_info(tenant_id, related_tenant_id, opts)

```ruby
begin
  # Sync a tenant into another tenant's contact list
  data, status_code, headers = api_instance.sync_tenant_to_tenant_crm_with_http_info(tenant_id, related_tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SyncApi->sync_tenant_to_tenant_crm_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **related_tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

