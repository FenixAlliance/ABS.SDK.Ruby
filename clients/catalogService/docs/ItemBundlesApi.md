# OpenapiClient::ItemBundlesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_bundle_async**](ItemBundlesApi.md#create_item_bundle_async) | **POST** /api/v2/CatalogService/ItemBundles | Create a new item bundle |
| [**delete_item_bundle_async**](ItemBundlesApi.md#delete_item_bundle_async) | **DELETE** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Delete an item bundle |
| [**get_item_bundle_by_id_async**](ItemBundlesApi.md#get_item_bundle_by_id_async) | **GET** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Get item bundle by ID |
| [**get_item_bundles_async**](ItemBundlesApi.md#get_item_bundles_async) | **GET** /api/v2/CatalogService/ItemBundles | Get all item bundles |
| [**get_item_bundles_count_async**](ItemBundlesApi.md#get_item_bundles_count_async) | **GET** /api/v2/CatalogService/ItemBundles/Count | Get item bundles count |
| [**patch_item_bundle_async**](ItemBundlesApi.md#patch_item_bundle_async) | **PATCH** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Patch an item bundle |
| [**update_item_bundle_async**](ItemBundlesApi.md#update_item_bundle_async) | **PUT** /api/v2/CatalogService/ItemBundles/{itemBundleId} | Update an item bundle |


## create_item_bundle_async

> <ItemBundleDtoEnvelope> create_item_bundle_async(tenant_id, opts)

Create a new item bundle

Creates a new item bundle for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_bundle_create_dto: OpenapiClient::ItemBundleCreateDto.new({name: 'name_example'}) # ItemBundleCreateDto | 
}

begin
  # Create a new item bundle
  result = api_instance.create_item_bundle_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->create_item_bundle_async: #{e}"
end
```

#### Using the create_item_bundle_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBundleDtoEnvelope>, Integer, Hash)> create_item_bundle_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item bundle
  data, status_code, headers = api_instance.create_item_bundle_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBundleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->create_item_bundle_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_bundle_create_dto** | [**ItemBundleCreateDto**](ItemBundleCreateDto.md) |  | [optional] |

### Return type

[**ItemBundleDtoEnvelope**](ItemBundleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_bundle_async

> delete_item_bundle_async(tenant_id, item_bundle_id, opts)

Delete an item bundle

Deletes an item bundle for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_bundle_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item bundle
  api_instance.delete_item_bundle_async(tenant_id, item_bundle_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->delete_item_bundle_async: #{e}"
end
```

#### Using the delete_item_bundle_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_bundle_async_with_http_info(tenant_id, item_bundle_id, opts)

```ruby
begin
  # Delete an item bundle
  data, status_code, headers = api_instance.delete_item_bundle_async_with_http_info(tenant_id, item_bundle_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->delete_item_bundle_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_bundle_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_bundle_by_id_async

> <ItemBundleDtoEnvelope> get_item_bundle_by_id_async(item_bundle_id, opts)

Get item bundle by ID

Retrieves a specific item bundle by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
item_bundle_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item bundle by ID
  result = api_instance.get_item_bundle_by_id_async(item_bundle_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->get_item_bundle_by_id_async: #{e}"
end
```

#### Using the get_item_bundle_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBundleDtoEnvelope>, Integer, Hash)> get_item_bundle_by_id_async_with_http_info(item_bundle_id, opts)

```ruby
begin
  # Get item bundle by ID
  data, status_code, headers = api_instance.get_item_bundle_by_id_async_with_http_info(item_bundle_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBundleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->get_item_bundle_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_bundle_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBundleDtoEnvelope**](ItemBundleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_bundles_async

> <ItemBundleDtoListEnvelope> get_item_bundles_async(opts)

Get all item bundles

Retrieves all item bundles for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_bundle_dto_collection_query_parameters: OpenapiClient::ItemBundleDtoCollectionQueryParameters.new # ItemBundleDtoCollectionQueryParameters | 
}

begin
  # Get all item bundles
  result = api_instance.get_item_bundles_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->get_item_bundles_async: #{e}"
end
```

#### Using the get_item_bundles_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBundleDtoListEnvelope>, Integer, Hash)> get_item_bundles_async_with_http_info(opts)

```ruby
begin
  # Get all item bundles
  data, status_code, headers = api_instance.get_item_bundles_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBundleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->get_item_bundles_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_bundle_dto_collection_query_parameters** | [**ItemBundleDtoCollectionQueryParameters**](ItemBundleDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemBundleDtoListEnvelope**](ItemBundleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_bundles_count_async

> <Int32Envelope> get_item_bundles_count_async(opts)

Get item bundles count

Returns the count of item bundles for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_bundle_dto_collection_query_parameters: OpenapiClient::ItemBundleDtoCollectionQueryParameters.new # ItemBundleDtoCollectionQueryParameters | 
}

begin
  # Get item bundles count
  result = api_instance.get_item_bundles_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->get_item_bundles_count_async: #{e}"
end
```

#### Using the get_item_bundles_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_bundles_count_async_with_http_info(opts)

```ruby
begin
  # Get item bundles count
  data, status_code, headers = api_instance.get_item_bundles_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->get_item_bundles_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_bundle_dto_collection_query_parameters** | [**ItemBundleDtoCollectionQueryParameters**](ItemBundleDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_item_bundle_async

> <EmptyEnvelope> patch_item_bundle_async(tenant_id, item_bundle_id, opts)

Patch an item bundle

Partially updates an existing item bundle for the specified tenant using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_bundle_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an item bundle
  result = api_instance.patch_item_bundle_async(tenant_id, item_bundle_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->patch_item_bundle_async: #{e}"
end
```

#### Using the patch_item_bundle_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_bundle_async_with_http_info(tenant_id, item_bundle_id, opts)

```ruby
begin
  # Patch an item bundle
  data, status_code, headers = api_instance.patch_item_bundle_async_with_http_info(tenant_id, item_bundle_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->patch_item_bundle_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_bundle_id** | **String** |  |  |
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


## update_item_bundle_async

> <ItemBundleDtoEnvelope> update_item_bundle_async(tenant_id, item_bundle_id, opts)

Update an item bundle

Updates an existing item bundle for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBundlesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_bundle_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_bundle_update_dto: OpenapiClient::ItemBundleUpdateDto.new({name: 'name_example'}) # ItemBundleUpdateDto | 
}

begin
  # Update an item bundle
  result = api_instance.update_item_bundle_async(tenant_id, item_bundle_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->update_item_bundle_async: #{e}"
end
```

#### Using the update_item_bundle_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBundleDtoEnvelope>, Integer, Hash)> update_item_bundle_async_with_http_info(tenant_id, item_bundle_id, opts)

```ruby
begin
  # Update an item bundle
  data, status_code, headers = api_instance.update_item_bundle_async_with_http_info(tenant_id, item_bundle_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBundleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBundlesApi->update_item_bundle_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_bundle_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_bundle_update_dto** | [**ItemBundleUpdateDto**](ItemBundleUpdateDto.md) |  | [optional] |

### Return type

[**ItemBundleDtoEnvelope**](ItemBundleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

