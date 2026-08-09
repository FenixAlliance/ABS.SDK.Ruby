# OpenapiClient::AssetTypesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_asset_type**](AssetTypesApi.md#create_asset_type) | **POST** /api/v2/AssetsService/AssetTypes | Creates a new asset type |
| [**delete_asset_type**](AssetTypesApi.md#delete_asset_type) | **DELETE** /api/v2/AssetsService/AssetTypes/{typeId} | Deletes an asset type |
| [**get_asset_type**](AssetTypesApi.md#get_asset_type) | **GET** /api/v2/AssetsService/AssetTypes/{typeId} | Gets a specific asset type |
| [**get_asset_types**](AssetTypesApi.md#get_asset_types) | **GET** /api/v2/AssetsService/AssetTypes | Gets all asset types for the current tenant |
| [**get_asset_types_count**](AssetTypesApi.md#get_asset_types_count) | **GET** /api/v2/AssetsService/AssetTypes/count | Gets the count of asset types |
| [**patch_asset_type**](AssetTypesApi.md#patch_asset_type) | **PATCH** /api/v2/AssetsService/AssetTypes/{typeId} | Partially updates an existing asset type |
| [**update_asset_type**](AssetTypesApi.md#update_asset_type) | **PUT** /api/v2/AssetsService/AssetTypes/{typeId} | Updates an existing asset type |


## create_asset_type

> <AssetTypeDtoEnvelope> create_asset_type(tenant_id, opts)

Creates a new asset type

Creates a new asset type for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_type_create_dto: OpenapiClient::AssetTypeCreateDto.new # AssetTypeCreateDto | 
}

begin
  # Creates a new asset type
  result = api_instance.create_asset_type(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->create_asset_type: #{e}"
end
```

#### Using the create_asset_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTypeDtoEnvelope>, Integer, Hash)> create_asset_type_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new asset type
  data, status_code, headers = api_instance.create_asset_type_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->create_asset_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_type_create_dto** | [**AssetTypeCreateDto**](AssetTypeCreateDto.md) |  | [optional] |

### Return type

[**AssetTypeDtoEnvelope**](AssetTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_asset_type

> delete_asset_type(tenant_id, type_id)

Deletes an asset type

Deletes an asset type for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an asset type
  api_instance.delete_asset_type(tenant_id, type_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->delete_asset_type: #{e}"
end
```

#### Using the delete_asset_type_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_asset_type_with_http_info(tenant_id, type_id)

```ruby
begin
  # Deletes an asset type
  data, status_code, headers = api_instance.delete_asset_type_with_http_info(tenant_id, type_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->delete_asset_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **type_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_type

> <AssetTypeDtoEnvelope> get_asset_type(tenant_id, type_id)

Gets a specific asset type

Retrieves a specific asset type by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific asset type
  result = api_instance.get_asset_type(tenant_id, type_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->get_asset_type: #{e}"
end
```

#### Using the get_asset_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTypeDtoEnvelope>, Integer, Hash)> get_asset_type_with_http_info(tenant_id, type_id)

```ruby
begin
  # Gets a specific asset type
  data, status_code, headers = api_instance.get_asset_type_with_http_info(tenant_id, type_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTypeDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->get_asset_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **type_id** | **String** |  |  |

### Return type

[**AssetTypeDtoEnvelope**](AssetTypeDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_types

> <AssetTypeDtoListEnvelope> get_asset_types(tenant_id, opts)

Gets all asset types for the current tenant

Retrieves all asset types for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_type_dto_collection_query_parameters: OpenapiClient::AssetTypeDtoCollectionQueryParameters.new # AssetTypeDtoCollectionQueryParameters | 
}

begin
  # Gets all asset types for the current tenant
  result = api_instance.get_asset_types(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->get_asset_types: #{e}"
end
```

#### Using the get_asset_types_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTypeDtoListEnvelope>, Integer, Hash)> get_asset_types_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all asset types for the current tenant
  data, status_code, headers = api_instance.get_asset_types_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTypeDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->get_asset_types_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_type_dto_collection_query_parameters** | [**AssetTypeDtoCollectionQueryParameters**](AssetTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetTypeDtoListEnvelope**](AssetTypeDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_types_count

> <Int32Envelope> get_asset_types_count(tenant_id, opts)

Gets the count of asset types

Returns the total number of asset types for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_type_dto_collection_query_parameters: OpenapiClient::AssetTypeDtoCollectionQueryParameters.new # AssetTypeDtoCollectionQueryParameters | 
}

begin
  # Gets the count of asset types
  result = api_instance.get_asset_types_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->get_asset_types_count: #{e}"
end
```

#### Using the get_asset_types_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_types_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the count of asset types
  data, status_code, headers = api_instance.get_asset_types_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->get_asset_types_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_type_dto_collection_query_parameters** | [**AssetTypeDtoCollectionQueryParameters**](AssetTypeDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_asset_type

> <EmptyEnvelope> patch_asset_type(tenant_id, type_id, opts)

Partially updates an existing asset type

Applies a JSON Patch document to an existing asset type for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates an existing asset type
  result = api_instance.patch_asset_type(tenant_id, type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->patch_asset_type: #{e}"
end
```

#### Using the patch_asset_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_type_with_http_info(tenant_id, type_id, opts)

```ruby
begin
  # Partially updates an existing asset type
  data, status_code, headers = api_instance.patch_asset_type_with_http_info(tenant_id, type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->patch_asset_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **type_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_type

> <EmptyEnvelope> update_asset_type(tenant_id, type_id, opts)

Updates an existing asset type

Updates an existing asset type for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTypesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
type_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_type_update_dto: OpenapiClient::AssetTypeUpdateDto.new # AssetTypeUpdateDto | 
}

begin
  # Updates an existing asset type
  result = api_instance.update_asset_type(tenant_id, type_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->update_asset_type: #{e}"
end
```

#### Using the update_asset_type_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_type_with_http_info(tenant_id, type_id, opts)

```ruby
begin
  # Updates an existing asset type
  data, status_code, headers = api_instance.update_asset_type_with_http_info(tenant_id, type_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTypesApi->update_asset_type_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **type_id** | **String** |  |  |
| **asset_type_update_dto** | [**AssetTypeUpdateDto**](AssetTypeUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

