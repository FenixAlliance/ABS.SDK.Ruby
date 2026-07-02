# OpenapiClient::ItemAttributesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_attributes_async**](ItemAttributesApi.md#count_item_attributes_async) | **GET** /api/v2/CatalogService/ItemAttributes/Count | Count item attributes |
| [**create_item_attribute_async**](ItemAttributesApi.md#create_item_attribute_async) | **POST** /api/v2/CatalogService/ItemAttributes | Create a new item attribute |
| [**delete_item_attribute_async**](ItemAttributesApi.md#delete_item_attribute_async) | **DELETE** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Delete an item attribute |
| [**get_item_attribute_by_id_async**](ItemAttributesApi.md#get_item_attribute_by_id_async) | **GET** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Get item attribute by ID |
| [**get_item_attributes_async**](ItemAttributesApi.md#get_item_attributes_async) | **GET** /api/v2/CatalogService/ItemAttributes | Get all item attributes |
| [**patch_item_attribute_async**](ItemAttributesApi.md#patch_item_attribute_async) | **PATCH** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Patch an item attribute |
| [**update_item_attribute_async**](ItemAttributesApi.md#update_item_attribute_async) | **PUT** /api/v2/CatalogService/ItemAttributes/{itemAttributeId} | Update an item attribute |


## count_item_attributes_async

> <Int32Envelope> count_item_attributes_async(opts)

Count item attributes

Counts all item attributes for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count item attributes
  result = api_instance.count_item_attributes_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->count_item_attributes_async: #{e}"
end
```

#### Using the count_item_attributes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_attributes_async_with_http_info(opts)

```ruby
begin
  # Count item attributes
  data, status_code, headers = api_instance.count_item_attributes_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->count_item_attributes_async_with_http_info: #{e}"
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


## create_item_attribute_async

> <ItemAttributeDtoEnvelope> create_item_attribute_async(tenant_id, opts)

Create a new item attribute

Creates a new item attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attribute_create_dto: OpenapiClient::ItemAttributeCreateDto.new({name: 'name_example'}) # ItemAttributeCreateDto | 
}

begin
  # Create a new item attribute
  result = api_instance.create_item_attribute_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->create_item_attribute_async: #{e}"
end
```

#### Using the create_item_attribute_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeDtoEnvelope>, Integer, Hash)> create_item_attribute_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item attribute
  data, status_code, headers = api_instance.create_item_attribute_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->create_item_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attribute_create_dto** | [**ItemAttributeCreateDto**](ItemAttributeCreateDto.md) |  | [optional] |

### Return type

[**ItemAttributeDtoEnvelope**](ItemAttributeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_attribute_async

> delete_item_attribute_async(tenant_id, item_attribute_id, opts)

Delete an item attribute

Deletes an item attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item attribute
  api_instance.delete_item_attribute_async(tenant_id, item_attribute_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->delete_item_attribute_async: #{e}"
end
```

#### Using the delete_item_attribute_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_attribute_async_with_http_info(tenant_id, item_attribute_id, opts)

```ruby
begin
  # Delete an item attribute
  data, status_code, headers = api_instance.delete_item_attribute_async_with_http_info(tenant_id, item_attribute_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->delete_item_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attribute_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attribute_by_id_async

> <ItemAttributeDtoEnvelope> get_item_attribute_by_id_async(item_attribute_id, opts)

Get item attribute by ID

Retrieves a specific item attribute by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
item_attribute_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item attribute by ID
  result = api_instance.get_item_attribute_by_id_async(item_attribute_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->get_item_attribute_by_id_async: #{e}"
end
```

#### Using the get_item_attribute_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeDtoEnvelope>, Integer, Hash)> get_item_attribute_by_id_async_with_http_info(item_attribute_id, opts)

```ruby
begin
  # Get item attribute by ID
  data, status_code, headers = api_instance.get_item_attribute_by_id_async_with_http_info(item_attribute_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->get_item_attribute_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_attribute_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeDtoEnvelope**](ItemAttributeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attributes_async

> <ItemAttributeDtoListEnvelope> get_item_attributes_async(opts)

Get all item attributes

Retrieves all item attributes for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item attributes
  result = api_instance.get_item_attributes_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->get_item_attributes_async: #{e}"
end
```

#### Using the get_item_attributes_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeDtoListEnvelope>, Integer, Hash)> get_item_attributes_async_with_http_info(opts)

```ruby
begin
  # Get all item attributes
  data, status_code, headers = api_instance.get_item_attributes_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->get_item_attributes_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeDtoListEnvelope**](ItemAttributeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_item_attribute_async

> patch_item_attribute_async(tenant_id, item_attribute_id, opts)

Patch an item attribute

Partially updates an existing item attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an item attribute
  api_instance.patch_item_attribute_async(tenant_id, item_attribute_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->patch_item_attribute_async: #{e}"
end
```

#### Using the patch_item_attribute_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_item_attribute_async_with_http_info(tenant_id, item_attribute_id, opts)

```ruby
begin
  # Patch an item attribute
  data, status_code, headers = api_instance.patch_item_attribute_async_with_http_info(tenant_id, item_attribute_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->patch_item_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attribute_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_attribute_async

> update_item_attribute_async(tenant_id, item_attribute_id, opts)

Update an item attribute

Updates an existing item attribute for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attribute_update_dto: OpenapiClient::ItemAttributeUpdateDto.new({name: 'name_example'}) # ItemAttributeUpdateDto | 
}

begin
  # Update an item attribute
  api_instance.update_item_attribute_async(tenant_id, item_attribute_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->update_item_attribute_async: #{e}"
end
```

#### Using the update_item_attribute_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_attribute_async_with_http_info(tenant_id, item_attribute_id, opts)

```ruby
begin
  # Update an item attribute
  data, status_code, headers = api_instance.update_item_attribute_async_with_http_info(tenant_id, item_attribute_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributesApi->update_item_attribute_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attribute_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attribute_update_dto** | [**ItemAttributeUpdateDto**](ItemAttributeUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

