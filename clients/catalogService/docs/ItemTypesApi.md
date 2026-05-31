# OpenapiClient::ItemTypesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_types_async**](ItemTypesApi.md#count_item_types_async) | **GET** /api/v2/CatalogService/ItemTypes/Count | Count item types |
| [**create_item_type_async**](ItemTypesApi.md#create_item_type_async) | **POST** /api/v2/CatalogService/ItemTypes | Create a new item type |
| [**delete_item_type_async**](ItemTypesApi.md#delete_item_type_async) | **DELETE** /api/v2/CatalogService/ItemTypes/{itemTypeID} | Delete an item type |
| [**get_item_type_by_id_async**](ItemTypesApi.md#get_item_type_by_id_async) | **GET** /api/v2/CatalogService/ItemTypes/{itemTypeID} | Get item type by ID |
| [**get_item_types_async**](ItemTypesApi.md#get_item_types_async) | **GET** /api/v2/CatalogService/ItemTypes | Get all item types |
| [**update_item_type_async**](ItemTypesApi.md#update_item_type_async) | **PUT** /api/v2/CatalogService/ItemTypes/{itemTypeID} | Update an item type |


## count_item_types_async

> <Int32Envelope> count_item_types_async(opts)

Count item types

Counts all item types for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTypesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item types
  result = api_instance.count_item_types_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->count_item_types_async: #{e}"
end
```

#### Using the count_item_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_types_async_with_http_info(opts)

```ruby
begin
  # Count item types
  data, status_code, headers = api_instance.count_item_types_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->count_item_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## create_item_type_async

> <ItemTypeDtoEnvelope> create_item_type_async(tenant_id, opts)

Create a new item type

Creates a new item type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_type_create_dto: OpenapiClient::ItemTypeCreateDto.new({item_category_id: 'item_category_id_example'}) # ItemTypeCreateDto | 
}

begin
  # Create a new item type
  result = api_instance.create_item_type_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->create_item_type_async: #{e}"
end
```

#### Using the create_item_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoEnvelope>, Integer, Hash)> create_item_type_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item type
  data, status_code, headers = api_instance.create_item_type_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->create_item_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_type_create_dto** | [**ItemTypeCreateDto**](ItemTypeCreateDto.md) |  | [optional] |

### Return type

[**ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_type_async

> <ItemTypeDtoEnvelope> delete_item_type_async(tenant_id, item_type_id, opts)

Delete an item type

Deletes an item type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item type
  result = api_instance.delete_item_type_async(tenant_id, item_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->delete_item_type_async: #{e}"
end
```

#### Using the delete_item_type_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoEnvelope>, Integer, Hash)> delete_item_type_async_with_http_info(tenant_id, item_type_id, opts)

```ruby
begin
  # Delete an item type
  data, status_code, headers = api_instance.delete_item_type_async_with_http_info(tenant_id, item_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->delete_item_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_type_by_id_async

> <ItemTypeDtoEnvelope> get_item_type_by_id_async(item_type_id, opts)

Get item type by ID

Retrieves a specific item type by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTypesApi.new
item_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item type by ID
  result = api_instance.get_item_type_by_id_async(item_type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->get_item_type_by_id_async: #{e}"
end
```

#### Using the get_item_type_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoEnvelope>, Integer, Hash)> get_item_type_by_id_async_with_http_info(item_type_id, opts)

```ruby
begin
  # Get item type by ID
  data, status_code, headers = api_instance.get_item_type_by_id_async_with_http_info(item_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->get_item_type_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_type_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoEnvelope**](ItemTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_types_async

> <ItemTypeDtoListEnvelope> get_item_types_async(opts)

Get all item types

Retrieves all item types for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTypesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item types
  result = api_instance.get_item_types_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->get_item_types_async: #{e}"
end
```

#### Using the get_item_types_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTypeDtoListEnvelope>, Integer, Hash)> get_item_types_async_with_http_info(opts)

```ruby
begin
  # Get all item types
  data, status_code, headers = api_instance.get_item_types_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->get_item_types_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTypeDtoListEnvelope**](ItemTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_type_async

> update_item_type_async(tenant_id, item_type_id, opts)

Update an item type

Updates an existing item type for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_type_update_dto: OpenapiClient::ItemTypeUpdateDto.new({singular_title: 'singular_title_example'}) # ItemTypeUpdateDto | 
}

begin
  # Update an item type
  api_instance.update_item_type_async(tenant_id, item_type_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->update_item_type_async: #{e}"
end
```

#### Using the update_item_type_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_type_async_with_http_info(tenant_id, item_type_id, opts)

```ruby
begin
  # Update an item type
  data, status_code, headers = api_instance.update_item_type_async_with_http_info(tenant_id, item_type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTypesApi->update_item_type_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_type_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_type_update_dto** | [**ItemTypeUpdateDto**](ItemTypeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

