# OpenapiClient::SizesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_tenant_size**](SizesApi.md#create_tenant_size) | **POST** /api/v2/TenantsService/Sizes | Create a new tenant size |
| [**delete_tenant_size**](SizesApi.md#delete_tenant_size) | **DELETE** /api/v2/TenantsService/Sizes/{tenantSizeId} | Delete a tenant size |
| [**get_tenant_size_by_id**](SizesApi.md#get_tenant_size_by_id) | **GET** /api/v2/TenantsService/Sizes/{tenantSizeId} | Retrieve a single tenant size by its ID |
| [**get_tenant_sizes**](SizesApi.md#get_tenant_sizes) | **GET** /api/v2/TenantsService/Sizes | Retrieve a list of tenant sizes |
| [**get_tenant_sizes_count**](SizesApi.md#get_tenant_sizes_count) | **GET** /api/v2/TenantsService/Sizes/Count | Get the count of tenant sizes |
| [**update_tenant_size**](SizesApi.md#update_tenant_size) | **PUT** /api/v2/TenantsService/Sizes/{tenantSizeId} | Update a tenant size |


## create_tenant_size

> <EmptyEnvelope> create_tenant_size(tenant_id, opts)

Create a new tenant size

Create a new tenant size

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SizesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_size_create_dto: OpenapiClient::TenantSizeCreateDto.new # TenantSizeCreateDto | 
}

begin
  # Create a new tenant size
  result = api_instance.create_tenant_size(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->create_tenant_size: #{e}"
end
```

#### Using the create_tenant_size_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_tenant_size_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new tenant size
  data, status_code, headers = api_instance.create_tenant_size_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->create_tenant_size_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_size_create_dto** | [**TenantSizeCreateDto**](TenantSizeCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_tenant_size

> <EmptyEnvelope> delete_tenant_size(tenant_id, tenant_size_id, opts)

Delete a tenant size

Delete a tenant size

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SizesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_size_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a tenant size
  result = api_instance.delete_tenant_size(tenant_id, tenant_size_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->delete_tenant_size: #{e}"
end
```

#### Using the delete_tenant_size_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_tenant_size_with_http_info(tenant_id, tenant_size_id, opts)

```ruby
begin
  # Delete a tenant size
  data, status_code, headers = api_instance.delete_tenant_size_with_http_info(tenant_id, tenant_size_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->delete_tenant_size_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_size_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_size_by_id

> <TenantSizeDtoEnvelope> get_tenant_size_by_id(tenant_id, tenant_size_id, opts)

Retrieve a single tenant size by its ID

Retrieve a single tenant size by its ID

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SizesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_size_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a single tenant size by its ID
  result = api_instance.get_tenant_size_by_id(tenant_id, tenant_size_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->get_tenant_size_by_id: #{e}"
end
```

#### Using the get_tenant_size_by_id_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantSizeDtoEnvelope>, Integer, Hash)> get_tenant_size_by_id_with_http_info(tenant_id, tenant_size_id, opts)

```ruby
begin
  # Retrieve a single tenant size by its ID
  data, status_code, headers = api_instance.get_tenant_size_by_id_with_http_info(tenant_id, tenant_size_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantSizeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->get_tenant_size_by_id_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_size_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantSizeDtoEnvelope**](TenantSizeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_sizes

> <TenantSizeDtoListEnvelope> get_tenant_sizes(tenant_id, opts)

Retrieve a list of tenant sizes

Retrieve a list of tenant sizes

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SizesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of tenant sizes
  result = api_instance.get_tenant_sizes(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->get_tenant_sizes: #{e}"
end
```

#### Using the get_tenant_sizes_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TenantSizeDtoListEnvelope>, Integer, Hash)> get_tenant_sizes_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of tenant sizes
  data, status_code, headers = api_instance.get_tenant_sizes_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TenantSizeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->get_tenant_sizes_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TenantSizeDtoListEnvelope**](TenantSizeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_tenant_sizes_count

> <Int32Envelope> get_tenant_sizes_count(tenant_id, opts)

Get the count of tenant sizes

Get the count of tenant sizes

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SizesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of tenant sizes
  result = api_instance.get_tenant_sizes_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->get_tenant_sizes_count: #{e}"
end
```

#### Using the get_tenant_sizes_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_tenant_sizes_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of tenant sizes
  data, status_code, headers = api_instance.get_tenant_sizes_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->get_tenant_sizes_count_with_http_info: #{e}"
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


## update_tenant_size

> <EmptyEnvelope> update_tenant_size(tenant_id, tenant_size_id, opts)

Update a tenant size

Update a tenant size

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SizesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
tenant_size_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  tenant_size_update_dto: OpenapiClient::TenantSizeUpdateDto.new # TenantSizeUpdateDto | 
}

begin
  # Update a tenant size
  result = api_instance.update_tenant_size(tenant_id, tenant_size_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->update_tenant_size: #{e}"
end
```

#### Using the update_tenant_size_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_tenant_size_with_http_info(tenant_id, tenant_size_id, opts)

```ruby
begin
  # Update a tenant size
  data, status_code, headers = api_instance.update_tenant_size_with_http_info(tenant_id, tenant_size_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SizesApi->update_tenant_size_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **tenant_size_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **tenant_size_update_dto** | [**TenantSizeUpdateDto**](TenantSizeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

