# OpenapiClient::WorkOrdersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_work_order_async**](WorkOrdersApi.md#create_work_order_async) | **POST** /api/v2/ManufacturingService/WorkOrders | Create a new work order |
| [**delete_work_order_async**](WorkOrdersApi.md#delete_work_order_async) | **DELETE** /api/v2/ManufacturingService/WorkOrders/{id} | Delete a work order |
| [**get_work_order_by_id_async**](WorkOrdersApi.md#get_work_order_by_id_async) | **GET** /api/v2/ManufacturingService/WorkOrders/{id} | Get work order by ID |
| [**get_work_orders_async**](WorkOrdersApi.md#get_work_orders_async) | **GET** /api/v2/ManufacturingService/WorkOrders | Get all work orders |
| [**get_work_orders_count_async**](WorkOrdersApi.md#get_work_orders_count_async) | **GET** /api/v2/ManufacturingService/WorkOrders/Count | Get work orders count |
| [**patch_work_order_async**](WorkOrdersApi.md#patch_work_order_async) | **PATCH** /api/v2/ManufacturingService/WorkOrders/{id} | Patch a work order |
| [**update_work_order_async**](WorkOrdersApi.md#update_work_order_async) | **PUT** /api/v2/ManufacturingService/WorkOrders/{id} | Update a work order |


## create_work_order_async

> create_work_order_async(tenant_id, opts)

Create a new work order

Creates a new work order for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_create_dto: OpenapiClient::WorkOrderCreateDto.new({title: 'title_example'}) # WorkOrderCreateDto | 
}

begin
  # Create a new work order
  api_instance.create_work_order_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->create_work_order_async: #{e}"
end
```

#### Using the create_work_order_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_work_order_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new work order
  data, status_code, headers = api_instance.create_work_order_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->create_work_order_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_create_dto** | [**WorkOrderCreateDto**](WorkOrderCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_work_order_async

> delete_work_order_async(tenant_id, id, opts)

Delete a work order

Deletes a work order for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a work order
  api_instance.delete_work_order_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->delete_work_order_async: #{e}"
end
```

#### Using the delete_work_order_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_work_order_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a work order
  data, status_code, headers = api_instance.delete_work_order_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->delete_work_order_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_work_order_by_id_async

> <WorkOrderDto> get_work_order_by_id_async(tenant_id, id, opts)

Get work order by ID

Retrieves a specific work order by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get work order by ID
  result = api_instance.get_work_order_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->get_work_order_by_id_async: #{e}"
end
```

#### Using the get_work_order_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WorkOrderDto>, Integer, Hash)> get_work_order_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get work order by ID
  data, status_code, headers = api_instance.get_work_order_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WorkOrderDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->get_work_order_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WorkOrderDto**](WorkOrderDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_work_orders_async

> <WorkOrderDtoListEnvelope> get_work_orders_async(tenant_id, opts)

Get all work orders

Retrieves all work orders for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_dto_collection_query_parameters: OpenapiClient::WorkOrderDtoCollectionQueryParameters.new # WorkOrderDtoCollectionQueryParameters | 
}

begin
  # Get all work orders
  result = api_instance.get_work_orders_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->get_work_orders_async: #{e}"
end
```

#### Using the get_work_orders_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WorkOrderDtoListEnvelope>, Integer, Hash)> get_work_orders_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all work orders
  data, status_code, headers = api_instance.get_work_orders_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WorkOrderDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->get_work_orders_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_dto_collection_query_parameters** | [**WorkOrderDtoCollectionQueryParameters**](WorkOrderDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WorkOrderDtoListEnvelope**](WorkOrderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_work_orders_count_async

> <Int32Envelope> get_work_orders_count_async(tenant_id, opts)

Get work orders count

Returns the count of work orders for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_dto_collection_query_parameters: OpenapiClient::WorkOrderDtoCollectionQueryParameters.new # WorkOrderDtoCollectionQueryParameters | 
}

begin
  # Get work orders count
  result = api_instance.get_work_orders_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->get_work_orders_count_async: #{e}"
end
```

#### Using the get_work_orders_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_work_orders_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get work orders count
  data, status_code, headers = api_instance.get_work_orders_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->get_work_orders_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_dto_collection_query_parameters** | [**WorkOrderDtoCollectionQueryParameters**](WorkOrderDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_work_order_async

> <EmptyEnvelope> patch_work_order_async(tenant_id, id, opts)

Patch a work order

Patch a work order

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a work order
  result = api_instance.patch_work_order_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->patch_work_order_async: #{e}"
end
```

#### Using the patch_work_order_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_work_order_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a work order
  data, status_code, headers = api_instance.patch_work_order_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->patch_work_order_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_work_order_async

> update_work_order_async(tenant_id, id, opts)

Update a work order

Updates an existing work order for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrdersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_update_dto: OpenapiClient::WorkOrderUpdateDto.new # WorkOrderUpdateDto | 
}

begin
  # Update a work order
  api_instance.update_work_order_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->update_work_order_async: #{e}"
end
```

#### Using the update_work_order_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_work_order_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a work order
  data, status_code, headers = api_instance.update_work_order_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrdersApi->update_work_order_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_update_dto** | [**WorkOrderUpdateDto**](WorkOrderUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

