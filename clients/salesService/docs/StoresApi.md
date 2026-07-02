# OpenapiClient::StoresApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_stores_async**](StoresApi.md#count_stores_async) | **GET** /api/v2/SalesService/Stores/Count | Get stores count |
| [**create_store_async**](StoresApi.md#create_store_async) | **POST** /api/v2/SalesService/Stores | Create a store |
| [**delete_store_async**](StoresApi.md#delete_store_async) | **DELETE** /api/v2/SalesService/Stores/{storeId} | Delete a store |
| [**get_store_async**](StoresApi.md#get_store_async) | **GET** /api/v2/SalesService/Stores/{storeId} | Get store by ID |
| [**get_stores_async**](StoresApi.md#get_stores_async) | **GET** /api/v2/SalesService/Stores | Get stores |
| [**patch_store_async**](StoresApi.md#patch_store_async) | **PATCH** /api/v2/SalesService/Stores/{storeId} | Patch a store |
| [**update_store_async**](StoresApi.md#update_store_async) | **PUT** /api/v2/SalesService/Stores/{storeId} | Update a store |


## count_stores_async

> <Int32Envelope> count_stores_async(tenant_id)

Get stores count

Returns the total count of stores for the specified tenant with OData filter support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get stores count
  result = api_instance.count_stores_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->count_stores_async: #{e}"
end
```

#### Using the count_stores_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_stores_async_with_http_info(tenant_id)

```ruby
begin
  # Get stores count
  data, status_code, headers = api_instance.count_stores_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->count_stores_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_store_async

> <EmptyEnvelope> create_store_async(tenant_id, opts)

Create a store

Creates a new store for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  store_create_dto: OpenapiClient::StoreCreateDto.new({name: 'name_example'}) # StoreCreateDto | 
}

begin
  # Create a store
  result = api_instance.create_store_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->create_store_async: #{e}"
end
```

#### Using the create_store_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_store_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a store
  data, status_code, headers = api_instance.create_store_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->create_store_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **store_create_dto** | [**StoreCreateDto**](StoreCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_store_async

> <EmptyEnvelope> delete_store_async(tenant_id, store_id)

Delete a store

Deletes an existing store by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete a store
  result = api_instance.delete_store_async(tenant_id, store_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->delete_store_async: #{e}"
end
```

#### Using the delete_store_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_store_async_with_http_info(tenant_id, store_id)

```ruby
begin
  # Delete a store
  data, status_code, headers = api_instance.delete_store_async_with_http_info(tenant_id, store_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->delete_store_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **store_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_store_async

> <StoreDtoEnvelope> get_store_async(tenant_id, store_id)

Get store by ID

Retrieves a single store by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get store by ID
  result = api_instance.get_store_async(tenant_id, store_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->get_store_async: #{e}"
end
```

#### Using the get_store_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreDtoEnvelope>, Integer, Hash)> get_store_async_with_http_info(tenant_id, store_id)

```ruby
begin
  # Get store by ID
  data, status_code, headers = api_instance.get_store_async_with_http_info(tenant_id, store_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->get_store_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **store_id** | **String** |  |  |

### Return type

[**StoreDtoEnvelope**](StoreDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_stores_async

> <StoreDtoListEnvelope> get_stores_async(tenant_id)

Get stores

Retrieves a list of stores for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get stores
  result = api_instance.get_stores_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->get_stores_async: #{e}"
end
```

#### Using the get_stores_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreDtoListEnvelope>, Integer, Hash)> get_stores_async_with_http_info(tenant_id)

```ruby
begin
  # Get stores
  data, status_code, headers = api_instance.get_stores_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->get_stores_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**StoreDtoListEnvelope**](StoreDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_store_async

> <EmptyEnvelope> patch_store_async(tenant_id, store_id, opts)

Patch a store

Partially updates an existing store using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a store
  result = api_instance.patch_store_async(tenant_id, store_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->patch_store_async: #{e}"
end
```

#### Using the patch_store_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_store_async_with_http_info(tenant_id, store_id, opts)

```ruby
begin
  # Patch a store
  data, status_code, headers = api_instance.patch_store_async_with_http_info(tenant_id, store_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->patch_store_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **store_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_store_async

> <EmptyEnvelope> update_store_async(tenant_id, store_id, opts)

Update a store

Updates an existing store by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::StoresApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  store_update_dto: OpenapiClient::StoreUpdateDto.new # StoreUpdateDto | 
}

begin
  # Update a store
  result = api_instance.update_store_async(tenant_id, store_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->update_store_async: #{e}"
end
```

#### Using the update_store_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_store_async_with_http_info(tenant_id, store_id, opts)

```ruby
begin
  # Update a store
  data, status_code, headers = api_instance.update_store_async_with_http_info(tenant_id, store_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StoresApi->update_store_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **store_id** | **String** |  |  |
| **store_update_dto** | [**StoreUpdateDto**](StoreUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

