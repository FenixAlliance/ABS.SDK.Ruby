# OpenapiClient::WarehousesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_warehouse_async**](WarehousesApi.md#create_warehouse_async) | **POST** /api/v2/LogisticsService/Warehouses | Create a warehouse |
| [**delete_warehouse_async**](WarehousesApi.md#delete_warehouse_async) | **DELETE** /api/v2/LogisticsService/Warehouses/{warehouseId} | Delete a warehouse |
| [**get_warehouse_by_id_async**](WarehousesApi.md#get_warehouse_by_id_async) | **GET** /api/v2/LogisticsService/Warehouses/{warehouseId} | Get warehouse by ID |
| [**get_warehouses_async**](WarehousesApi.md#get_warehouses_async) | **GET** /api/v2/LogisticsService/Warehouses | Get all warehouses |
| [**get_warehouses_count_async**](WarehousesApi.md#get_warehouses_count_async) | **GET** /api/v2/LogisticsService/Warehouses/Count | Get warehouses count |
| [**patch_warehouse_async**](WarehousesApi.md#patch_warehouse_async) | **PATCH** /api/v2/LogisticsService/Warehouses/{warehouseId} | Patch a warehouse |
| [**update_warehouse_async**](WarehousesApi.md#update_warehouse_async) | **PUT** /api/v2/LogisticsService/Warehouses/{warehouseId} | Update a warehouse |


## create_warehouse_async

> <EmptyEnvelope> create_warehouse_async(tenant_id, opts)

Create a warehouse

Creates a new warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warehouse_create_dto: OpenapiClient::WarehouseCreateDto.new({title: 'title_example', address1: 'address1_example'}) # WarehouseCreateDto | 
}

begin
  # Create a warehouse
  result = api_instance.create_warehouse_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->create_warehouse_async: #{e}"
end
```

#### Using the create_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_warehouse_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a warehouse
  data, status_code, headers = api_instance.create_warehouse_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->create_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warehouse_create_dto** | [**WarehouseCreateDto**](WarehouseCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_warehouse_async

> <EmptyEnvelope> delete_warehouse_async(tenant_id, warehouse_id, opts)

Delete a warehouse

Deletes a warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a warehouse
  result = api_instance.delete_warehouse_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->delete_warehouse_async: #{e}"
end
```

#### Using the delete_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Delete a warehouse
  data, status_code, headers = api_instance.delete_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->delete_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warehouse_by_id_async

> <WarehouseDtoEnvelope> get_warehouse_by_id_async(tenant_id, warehouse_id, opts)

Get warehouse by ID

Retrieves a specific warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warehouse by ID
  result = api_instance.get_warehouse_by_id_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->get_warehouse_by_id_async: #{e}"
end
```

#### Using the get_warehouse_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarehouseDtoEnvelope>, Integer, Hash)> get_warehouse_by_id_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Get warehouse by ID
  data, status_code, headers = api_instance.get_warehouse_by_id_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarehouseDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->get_warehouse_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarehouseDtoEnvelope**](WarehouseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warehouses_async

> <WarehouseDtoListEnvelope> get_warehouses_async(tenant_id, opts)

Get all warehouses

Retrieves all warehouses for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all warehouses
  result = api_instance.get_warehouses_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->get_warehouses_async: #{e}"
end
```

#### Using the get_warehouses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarehouseDtoListEnvelope>, Integer, Hash)> get_warehouses_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all warehouses
  data, status_code, headers = api_instance.get_warehouses_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarehouseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->get_warehouses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarehouseDtoListEnvelope**](WarehouseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warehouses_count_async

> <Int32Envelope> get_warehouses_count_async(tenant_id, opts)

Get warehouses count

Returns the count of warehouses.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warehouses count
  result = api_instance.get_warehouses_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->get_warehouses_count_async: #{e}"
end
```

#### Using the get_warehouses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_warehouses_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get warehouses count
  data, status_code, headers = api_instance.get_warehouses_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->get_warehouses_count_async_with_http_info: #{e}"
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


## patch_warehouse_async

> <EmptyEnvelope> patch_warehouse_async(tenant_id, warehouse_id, opts)

Patch a warehouse

Partially updates an existing warehouse using JSON Patch.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a warehouse
  result = api_instance.patch_warehouse_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->patch_warehouse_async: #{e}"
end
```

#### Using the patch_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Patch a warehouse
  data, status_code, headers = api_instance.patch_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->patch_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
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


## update_warehouse_async

> <EmptyEnvelope> update_warehouse_async(tenant_id, warehouse_id, opts)

Update a warehouse

Updates an existing warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warehouse_update_dto: OpenapiClient::WarehouseUpdateDto.new # WarehouseUpdateDto | 
}

begin
  # Update a warehouse
  result = api_instance.update_warehouse_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->update_warehouse_async: #{e}"
end
```

#### Using the update_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Update a warehouse
  data, status_code, headers = api_instance.update_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousesApi->update_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warehouse_update_dto** | [**WarehouseUpdateDto**](WarehouseUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

