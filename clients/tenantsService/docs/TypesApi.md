# OpenapiClient::TypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_type**](TypesApi.md#create_tenant_type) | **POST** /api/v2/TenantsService/Types | Create a new tenant type |
| [**delete_tenant_type**](TypesApi.md#delete_tenant_type) | **DELETE** /api/v2/TenantsService/Types/{tenantTypeId} | Delete a tenant type |
| [**get_tenant_type_by_id**](TypesApi.md#get_tenant_type_by_id) | **GET** /api/v2/TenantsService/Types/{tenantTypeId} | Retrieve a single tenant type by its ID |
| [**get_tenant_types**](TypesApi.md#get_tenant_types) | **GET** /api/v2/TenantsService/Types | Retrieve a list of tenant types |
| [**get_tenant_types_count**](TypesApi.md#get_tenant_types_count) | **GET** /api/v2/TenantsService/Types/Count | Get the count of tenant types |
| [**patch_tenant_type**](TypesApi.md#patch_tenant_type) | **PATCH** /api/v2/TenantsService/Types/{tenantTypeId} | Patch a tenant type |
| [**update_tenant_type**](TypesApi.md#update_tenant_type) | **PUT** /api/v2/TenantsService/Types/{tenantTypeId} | Update a tenant type |


## create_tenant_type

> <EmptyEnvelope> create_tenant_type(tenant_id, opts)

Create a new tenant type

Create a new tenant type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_type_create_dto: OpenapiClient::TenantTypeCreateDto.new # TenantTypeCreateDto | 
}

begin
  # Create a new tenant type
  result = api_instance.create_tenant_type(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->create_tenant_type: #{e}"
end
```

#### Using the create_tenant_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_type_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant type
  data, status_code, headers = api_instance.create_tenant_type_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->create_tenant_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_type_create_dto** | [**TenantTypeCreateDto**](TenantTypeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_type

> <EmptyEnvelope> delete_tenant_type(tenant_id, tenant_type_id, opts)

Delete a tenant type

Delete a tenant type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant type
  result = api_instance.delete_tenant_type(tenant_id, tenant_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->delete_tenant_type: #{e}"
end
```

#### Using the delete_tenant_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_type_with_http_info(tenant_id, tenant_type_id, opts)

```ruby
begin
  # Delete a tenant type
  data, status_code, headers = api_instance.delete_tenant_type_with_http_info(tenant_id, tenant_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->delete_tenant_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_type_by_id

> <TenantTypeDtoEnvelope> get_tenant_type_by_id(tenant_id, tenant_type_id, opts)

Retrieve a single tenant type by its ID

Retrieve a single tenant type by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant type by its ID
  result = api_instance.get_tenant_type_by_id(tenant_id, tenant_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->get_tenant_type_by_id: #{e}"
end
```

#### Using the get_tenant_type_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTypeDtoEnvelope>, Integer, Hash)> get_tenant_type_by_id_with_http_info(tenant_id, tenant_type_id, opts)

```ruby
begin
  # Retrieve a single tenant type by its ID
  data, status_code, headers = api_instance.get_tenant_type_by_id_with_http_info(tenant_id, tenant_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->get_tenant_type_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTypeDtoEnvelope**](TenantTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_types

> <TenantTypeDtoListEnvelope> get_tenant_types(tenant_id, opts)

Retrieve a list of tenant types

Retrieve a list of tenant types

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant types
  result = api_instance.get_tenant_types(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->get_tenant_types: #{e}"
end
```

#### Using the get_tenant_types_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantTypeDtoListEnvelope>, Integer, Hash)> get_tenant_types_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant types
  data, status_code, headers = api_instance.get_tenant_types_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->get_tenant_types_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantTypeDtoListEnvelope**](TenantTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_types_count

> <Int32Envelope> get_tenant_types_count(tenant_id, opts)

Get the count of tenant types

Get the count of tenant types

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant types
  result = api_instance.get_tenant_types_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->get_tenant_types_count: #{e}"
end
```

#### Using the get_tenant_types_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_types_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant types
  data, status_code, headers = api_instance.get_tenant_types_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->get_tenant_types_count_with_http_info: #{e}"
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


## patch_tenant_type

> <EmptyEnvelope> patch_tenant_type(tenant_id, tenant_type_id, opts)

Patch a tenant type

Patch a tenant type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a tenant type
  result = api_instance.patch_tenant_type(tenant_id, tenant_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->patch_tenant_type: #{e}"
end
```

#### Using the patch_tenant_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_tenant_type_with_http_info(tenant_id, tenant_type_id, opts)

```ruby
begin
  # Patch a tenant type
  data, status_code, headers = api_instance.patch_tenant_type_with_http_info(tenant_id, tenant_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->patch_tenant_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_type_id** | **String** |  |  |
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


## update_tenant_type

> <EmptyEnvelope> update_tenant_type(tenant_id, tenant_type_id, opts)

Update a tenant type

Update a tenant type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_type_update_dto: OpenapiClient::TenantTypeUpdateDto.new # TenantTypeUpdateDto | 
}

begin
  # Update a tenant type
  result = api_instance.update_tenant_type(tenant_id, tenant_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->update_tenant_type: #{e}"
end
```

#### Using the update_tenant_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_type_with_http_info(tenant_id, tenant_type_id, opts)

```ruby
begin
  # Update a tenant type
  data, status_code, headers = api_instance.update_tenant_type_with_http_info(tenant_id, tenant_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TypesApi->update_tenant_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_type_update_dto** | [**TenantTypeUpdateDto**](TenantTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

