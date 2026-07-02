# OpenapiClient::SupportEntitlementsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_support_entitlement_async**](SupportEntitlementsApi.md#create_support_entitlement_async) | **POST** /api/v2/SupportService/SupportEntitlements | Create a new support entitlement |
| [**delete_support_entitlement_async**](SupportEntitlementsApi.md#delete_support_entitlement_async) | **DELETE** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Delete a support entitlement |
| [**get_support_entitlement_async**](SupportEntitlementsApi.md#get_support_entitlement_async) | **GET** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Retrieve a support entitlement by ID |
| [**get_support_entitlements_async**](SupportEntitlementsApi.md#get_support_entitlements_async) | **GET** /api/v2/SupportService/SupportEntitlements | Retrieve a list of support entitlements |
| [**get_support_entitlements_count_async**](SupportEntitlementsApi.md#get_support_entitlements_count_async) | **GET** /api/v2/SupportService/SupportEntitlements/Count | Get the count of support entitlements |
| [**patch_support_entitlement_async**](SupportEntitlementsApi.md#patch_support_entitlement_async) | **PATCH** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Patch a support entitlement |
| [**update_support_entitlement_async**](SupportEntitlementsApi.md#update_support_entitlement_async) | **PUT** /api/v2/SupportService/SupportEntitlements/{supportEntitlementId} | Update a support entitlement |


## create_support_entitlement_async

> <EmptyEnvelope> create_support_entitlement_async(tenant_id, opts)

Create a new support entitlement

Creates a new support entitlement for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_entitlement_create_dto: OpenapiClient::SupportEntitlementCreateDto.new # SupportEntitlementCreateDto | 
}

begin
  # Create a new support entitlement
  result = api_instance.create_support_entitlement_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->create_support_entitlement_async: #{e}"
end
```

#### Using the create_support_entitlement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_support_entitlement_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new support entitlement
  data, status_code, headers = api_instance.create_support_entitlement_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->create_support_entitlement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_entitlement_create_dto** | [**SupportEntitlementCreateDto**](SupportEntitlementCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_support_entitlement_async

> <EmptyEnvelope> delete_support_entitlement_async(tenant_id, support_entitlement_id, opts)

Delete a support entitlement

Deletes a support entitlement by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_entitlement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a support entitlement
  result = api_instance.delete_support_entitlement_async(tenant_id, support_entitlement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->delete_support_entitlement_async: #{e}"
end
```

#### Using the delete_support_entitlement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)

```ruby
begin
  # Delete a support entitlement
  data, status_code, headers = api_instance.delete_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->delete_support_entitlement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_entitlement_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_entitlement_async

> <SupportEntitlementDtoEnvelope> get_support_entitlement_async(tenant_id, support_entitlement_id, opts)

Retrieve a support entitlement by ID

Retrieves a single support entitlement by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_entitlement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a support entitlement by ID
  result = api_instance.get_support_entitlement_async(tenant_id, support_entitlement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->get_support_entitlement_async: #{e}"
end
```

#### Using the get_support_entitlement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportEntitlementDtoEnvelope>, Integer, Hash)> get_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)

```ruby
begin
  # Retrieve a support entitlement by ID
  data, status_code, headers = api_instance.get_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportEntitlementDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->get_support_entitlement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_entitlement_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportEntitlementDtoEnvelope**](SupportEntitlementDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_entitlements_async

> <SupportEntitlementDtoListEnvelope> get_support_entitlements_async(tenant_id, opts)

Retrieve a list of support entitlements

Retrieves a list of support entitlements for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of support entitlements
  result = api_instance.get_support_entitlements_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->get_support_entitlements_async: #{e}"
end
```

#### Using the get_support_entitlements_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportEntitlementDtoListEnvelope>, Integer, Hash)> get_support_entitlements_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of support entitlements
  data, status_code, headers = api_instance.get_support_entitlements_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportEntitlementDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->get_support_entitlements_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportEntitlementDtoListEnvelope**](SupportEntitlementDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_entitlements_count_async

> <Int32Envelope> get_support_entitlements_count_async(tenant_id, opts)

Get the count of support entitlements

Returns the total count of support entitlements for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of support entitlements
  result = api_instance.get_support_entitlements_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->get_support_entitlements_count_async: #{e}"
end
```

#### Using the get_support_entitlements_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_entitlements_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of support entitlements
  data, status_code, headers = api_instance.get_support_entitlements_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->get_support_entitlements_count_async_with_http_info: #{e}"
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


## patch_support_entitlement_async

> <EmptyEnvelope> patch_support_entitlement_async(tenant_id, support_entitlement_id, opts)

Patch a support entitlement

Partially updates an existing support entitlement by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_entitlement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a support entitlement
  result = api_instance.patch_support_entitlement_async(tenant_id, support_entitlement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->patch_support_entitlement_async: #{e}"
end
```

#### Using the patch_support_entitlement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)

```ruby
begin
  # Patch a support entitlement
  data, status_code, headers = api_instance.patch_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->patch_support_entitlement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_entitlement_id** | **String** |  |  |
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


## update_support_entitlement_async

> <EmptyEnvelope> update_support_entitlement_async(tenant_id, support_entitlement_id, opts)

Update a support entitlement

Updates an existing support entitlement by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportEntitlementsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_entitlement_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_entitlement_update_dto: OpenapiClient::SupportEntitlementUpdateDto.new # SupportEntitlementUpdateDto | 
}

begin
  # Update a support entitlement
  result = api_instance.update_support_entitlement_async(tenant_id, support_entitlement_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->update_support_entitlement_async: #{e}"
end
```

#### Using the update_support_entitlement_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)

```ruby
begin
  # Update a support entitlement
  data, status_code, headers = api_instance.update_support_entitlement_async_with_http_info(tenant_id, support_entitlement_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportEntitlementsApi->update_support_entitlement_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_entitlement_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_entitlement_update_dto** | [**SupportEntitlementUpdateDto**](SupportEntitlementUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

