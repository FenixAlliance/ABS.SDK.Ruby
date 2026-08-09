# OpenapiClient::WorkOrderTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_work_order_type_async**](WorkOrderTypesApi.md#create_work_order_type_async) | **POST** /api/v2/ManufacturingService/WorkOrderTypes | Create a new work order type |
| [**delete_work_order_type_async**](WorkOrderTypesApi.md#delete_work_order_type_async) | **DELETE** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Delete a work order type |
| [**get_work_order_type_by_id_async**](WorkOrderTypesApi.md#get_work_order_type_by_id_async) | **GET** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Get work order type by ID |
| [**get_work_order_types_async**](WorkOrderTypesApi.md#get_work_order_types_async) | **GET** /api/v2/ManufacturingService/WorkOrderTypes | Get all work order types |
| [**get_work_order_types_count_async**](WorkOrderTypesApi.md#get_work_order_types_count_async) | **GET** /api/v2/ManufacturingService/WorkOrderTypes/Count | Get work order types count |
| [**patch_work_order_type_async**](WorkOrderTypesApi.md#patch_work_order_type_async) | **PATCH** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Patch a work order type |
| [**update_work_order_type_async**](WorkOrderTypesApi.md#update_work_order_type_async) | **PUT** /api/v2/ManufacturingService/WorkOrderTypes/{id} | Update a work order type |


## create_work_order_type_async

> create_work_order_type_async(tenant_id, opts)

Create a new work order type

Creates a new work order type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_type_create_dto: OpenapiClient::WorkOrderTypeCreateDto.new({name: 'name_example'}) # WorkOrderTypeCreateDto | 
}

begin
  # Create a new work order type
  api_instance.create_work_order_type_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->create_work_order_type_async: #{e}"
end
```

#### Using the create_work_order_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_work_order_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new work order type
  data, status_code, headers = api_instance.create_work_order_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->create_work_order_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_type_create_dto** | [**WorkOrderTypeCreateDto**](WorkOrderTypeCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_work_order_type_async

> delete_work_order_type_async(tenant_id, id, opts)

Delete a work order type

Deletes a work order type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a work order type
  api_instance.delete_work_order_type_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->delete_work_order_type_async: #{e}"
end
```

#### Using the delete_work_order_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_work_order_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a work order type
  data, status_code, headers = api_instance.delete_work_order_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->delete_work_order_type_async_with_http_info: #{e}"
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


## get_work_order_type_by_id_async

> <WorkOrderTypeDto> get_work_order_type_by_id_async(tenant_id, id, opts)

Get work order type by ID

Retrieves a specific work order type by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get work order type by ID
  result = api_instance.get_work_order_type_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->get_work_order_type_by_id_async: #{e}"
end
```

#### Using the get_work_order_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WorkOrderTypeDto>, Integer, Hash)> get_work_order_type_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get work order type by ID
  data, status_code, headers = api_instance.get_work_order_type_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WorkOrderTypeDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->get_work_order_type_by_id_async_with_http_info: #{e}"
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

[**WorkOrderTypeDto**](WorkOrderTypeDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_work_order_types_async

> <WorkOrderTypeDtoListEnvelope> get_work_order_types_async(tenant_id, opts)

Get all work order types

Retrieves all work order types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_type_dto_collection_query_parameters: OpenapiClient::WorkOrderTypeDtoCollectionQueryParameters.new # WorkOrderTypeDtoCollectionQueryParameters | 
}

begin
  # Get all work order types
  result = api_instance.get_work_order_types_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->get_work_order_types_async: #{e}"
end
```

#### Using the get_work_order_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WorkOrderTypeDtoListEnvelope>, Integer, Hash)> get_work_order_types_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all work order types
  data, status_code, headers = api_instance.get_work_order_types_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WorkOrderTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->get_work_order_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_type_dto_collection_query_parameters** | [**WorkOrderTypeDtoCollectionQueryParameters**](WorkOrderTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**WorkOrderTypeDtoListEnvelope**](WorkOrderTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_work_order_types_count_async

> <Int32Envelope> get_work_order_types_count_async(tenant_id, opts)

Get work order types count

Returns the count of work order types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_type_dto_collection_query_parameters: OpenapiClient::WorkOrderTypeDtoCollectionQueryParameters.new # WorkOrderTypeDtoCollectionQueryParameters | 
}

begin
  # Get work order types count
  result = api_instance.get_work_order_types_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->get_work_order_types_count_async: #{e}"
end
```

#### Using the get_work_order_types_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_work_order_types_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get work order types count
  data, status_code, headers = api_instance.get_work_order_types_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->get_work_order_types_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_type_dto_collection_query_parameters** | [**WorkOrderTypeDtoCollectionQueryParameters**](WorkOrderTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_work_order_type_async

> <EmptyEnvelope> patch_work_order_type_async(tenant_id, id, opts)

Patch a work order type

Patch a work order type

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a work order type
  result = api_instance.patch_work_order_type_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->patch_work_order_type_async: #{e}"
end
```

#### Using the patch_work_order_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_work_order_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a work order type
  data, status_code, headers = api_instance.patch_work_order_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->patch_work_order_type_async_with_http_info: #{e}"
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


## update_work_order_type_async

> update_work_order_type_async(tenant_id, id, opts)

Update a work order type

Updates an existing work order type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WorkOrderTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  work_order_type_update_dto: OpenapiClient::WorkOrderTypeUpdateDto.new # WorkOrderTypeUpdateDto | 
}

begin
  # Update a work order type
  api_instance.update_work_order_type_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->update_work_order_type_async: #{e}"
end
```

#### Using the update_work_order_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_work_order_type_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a work order type
  data, status_code, headers = api_instance.update_work_order_type_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WorkOrderTypesApi->update_work_order_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **work_order_type_update_dto** | [**WorkOrderTypeUpdateDto**](WorkOrderTypeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

