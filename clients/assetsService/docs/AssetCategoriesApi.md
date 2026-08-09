# OpenapiClient::AssetCategoriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_asset_category**](AssetCategoriesApi.md#create_asset_category) | **POST** /api/v2/AssetsService/AssetCategories | Creates a new asset category |
| [**delete_asset_category**](AssetCategoriesApi.md#delete_asset_category) | **DELETE** /api/v2/AssetsService/AssetCategories/{categoryId} | Deletes an asset category |
| [**get_asset_categories**](AssetCategoriesApi.md#get_asset_categories) | **GET** /api/v2/AssetsService/AssetCategories | Gets all asset categories for the current tenant |
| [**get_asset_categories_count**](AssetCategoriesApi.md#get_asset_categories_count) | **GET** /api/v2/AssetsService/AssetCategories/count | Gets the count of asset categories |
| [**get_asset_category**](AssetCategoriesApi.md#get_asset_category) | **GET** /api/v2/AssetsService/AssetCategories/{categoryId} | Gets a specific asset category |
| [**patch_asset_category**](AssetCategoriesApi.md#patch_asset_category) | **PATCH** /api/v2/AssetsService/AssetCategories/{categoryId} | Partially updates an existing asset category |
| [**update_asset_category**](AssetCategoriesApi.md#update_asset_category) | **PUT** /api/v2/AssetsService/AssetCategories/{categoryId} | Updates an existing asset category |


## create_asset_category

> <AssetCategoryDtoEnvelope> create_asset_category(tenant_id, opts)

Creates a new asset category

Creates a new asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_create_dto: OpenapiClient::AssetCategoryCreateDto.new # AssetCategoryCreateDto | 
}

begin
  # Creates a new asset category
  result = api_instance.create_asset_category(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->create_asset_category: #{e}"
end
```

#### Using the create_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoEnvelope>, Integer, Hash)> create_asset_category_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new asset category
  data, status_code, headers = api_instance.create_asset_category_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->create_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_category_create_dto** | [**AssetCategoryCreateDto**](AssetCategoryCreateDto.md) |  | [optional] |

### Return type

[**AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_asset_category

> delete_asset_category(tenant_id, category_id)

Deletes an asset category

Deletes an asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an asset category
  api_instance.delete_asset_category(tenant_id, category_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->delete_asset_category: #{e}"
end
```

#### Using the delete_asset_category_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_asset_category_with_http_info(tenant_id, category_id)

```ruby
begin
  # Deletes an asset category
  data, status_code, headers = api_instance.delete_asset_category_with_http_info(tenant_id, category_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->delete_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_categories

> <AssetCategoryDtoListEnvelope> get_asset_categories(tenant_id, opts)

Gets all asset categories for the current tenant

Retrieves all asset categories for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_dto_collection_query_parameters: OpenapiClient::AssetCategoryDtoCollectionQueryParameters.new # AssetCategoryDtoCollectionQueryParameters | 
}

begin
  # Gets all asset categories for the current tenant
  result = api_instance.get_asset_categories(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->get_asset_categories: #{e}"
end
```

#### Using the get_asset_categories_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoListEnvelope>, Integer, Hash)> get_asset_categories_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets all asset categories for the current tenant
  data, status_code, headers = api_instance.get_asset_categories_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->get_asset_categories_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_category_dto_collection_query_parameters** | [**AssetCategoryDtoCollectionQueryParameters**](AssetCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**AssetCategoryDtoListEnvelope**](AssetCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_categories_count

> <Int32Envelope> get_asset_categories_count(tenant_id, opts)

Gets the count of asset categories

Returns the total number of asset categories for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_dto_collection_query_parameters: OpenapiClient::AssetCategoryDtoCollectionQueryParameters.new # AssetCategoryDtoCollectionQueryParameters | 
}

begin
  # Gets the count of asset categories
  result = api_instance.get_asset_categories_count(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->get_asset_categories_count: #{e}"
end
```

#### Using the get_asset_categories_count_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_categories_count_with_http_info(tenant_id, opts)

```ruby
begin
  # Gets the count of asset categories
  data, status_code, headers = api_instance.get_asset_categories_count_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->get_asset_categories_count_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_category_dto_collection_query_parameters** | [**AssetCategoryDtoCollectionQueryParameters**](AssetCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_asset_category

> <AssetCategoryDtoEnvelope> get_asset_category(tenant_id, category_id)

Gets a specific asset category

Retrieves a specific asset category by ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a specific asset category
  result = api_instance.get_asset_category(tenant_id, category_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->get_asset_category: #{e}"
end
```

#### Using the get_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetCategoryDtoEnvelope>, Integer, Hash)> get_asset_category_with_http_info(tenant_id, category_id)

```ruby
begin
  # Gets a specific asset category
  data, status_code, headers = api_instance.get_asset_category_with_http_info(tenant_id, category_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->get_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |

### Return type

[**AssetCategoryDtoEnvelope**](AssetCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_asset_category

> <EmptyEnvelope> patch_asset_category(tenant_id, category_id, opts)

Partially updates an existing asset category

Applies a JSON Patch document to an existing asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Partially updates an existing asset category
  result = api_instance.patch_asset_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->patch_asset_category: #{e}"
end
```

#### Using the patch_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Partially updates an existing asset category
  data, status_code, headers = api_instance.patch_asset_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->patch_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_category

> <EmptyEnvelope> update_asset_category(tenant_id, category_id, opts)

Updates an existing asset category

Updates an existing asset category for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_category_update_dto: OpenapiClient::AssetCategoryUpdateDto.new # AssetCategoryUpdateDto | 
}

begin
  # Updates an existing asset category
  result = api_instance.update_asset_category(tenant_id, category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->update_asset_category: #{e}"
end
```

#### Using the update_asset_category_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_category_with_http_info(tenant_id, category_id, opts)

```ruby
begin
  # Updates an existing asset category
  data, status_code, headers = api_instance.update_asset_category_with_http_info(tenant_id, category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetCategoriesApi->update_asset_category_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **category_id** | **String** |  |  |
| **asset_category_update_dto** | [**AssetCategoryUpdateDto**](AssetCategoryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

