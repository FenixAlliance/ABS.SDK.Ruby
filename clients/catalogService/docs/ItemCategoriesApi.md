# OpenapiClient::ItemCategoriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_item_categories_async**](ItemCategoriesApi.md#count_item_categories_async) | **GET** /api/v2/CatalogService/ItemCategories/Count | Count item categories |
| [**create_item_category_async**](ItemCategoriesApi.md#create_item_category_async) | **POST** /api/v2/CatalogService/ItemCategories | Create a new item category |
| [**delete_item_category_async**](ItemCategoriesApi.md#delete_item_category_async) | **DELETE** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Delete an item category |
| [**get_item_categories_async**](ItemCategoriesApi.md#get_item_categories_async) | **GET** /api/v2/CatalogService/ItemCategories | Get all item categories |
| [**get_item_category_by_id_async**](ItemCategoriesApi.md#get_item_category_by_id_async) | **GET** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Get item category by ID |
| [**patch_item_category_async**](ItemCategoriesApi.md#patch_item_category_async) | **PATCH** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Patch an item category |
| [**update_item_category_async**](ItemCategoriesApi.md#update_item_category_async) | **PUT** /api/v2/CatalogService/ItemCategories/{itemCategoryId} | Update an item category |


## count_item_categories_async

> <Int32Envelope> count_item_categories_async(opts)

Count item categories

Counts all item categories for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_category_dto_collection_query_parameters: OpenapiClient::ItemCategoryDtoCollectionQueryParameters.new # ItemCategoryDtoCollectionQueryParameters | 
}

begin
  # Count item categories
  result = api_instance.count_item_categories_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->count_item_categories_async: #{e}"
end
```

#### Using the count_item_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_item_categories_async_with_http_info(opts)

```ruby
begin
  # Count item categories
  data, status_code, headers = api_instance.count_item_categories_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->count_item_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_category_dto_collection_query_parameters** | [**ItemCategoryDtoCollectionQueryParameters**](ItemCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_item_category_async

> <ItemCategoryDtoEnvelope> create_item_category_async(tenant_id, opts)

Create a new item category

Creates a new item category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_category_create_dto: OpenapiClient::ItemCategoryCreateDto.new({title: 'title_example'}) # ItemCategoryCreateDto | 
}

begin
  # Create a new item category
  result = api_instance.create_item_category_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->create_item_category_async: #{e}"
end
```

#### Using the create_item_category_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoEnvelope>, Integer, Hash)> create_item_category_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item category
  data, status_code, headers = api_instance.create_item_category_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->create_item_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_category_create_dto** | [**ItemCategoryCreateDto**](ItemCategoryCreateDto.md) |  | [optional] |

### Return type

[**ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_category_async

> delete_item_category_async(tenant_id, item_category_id, opts)

Delete an item category

Deletes an item category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item category
  api_instance.delete_item_category_async(tenant_id, item_category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->delete_item_category_async: #{e}"
end
```

#### Using the delete_item_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_category_async_with_http_info(tenant_id, item_category_id, opts)

```ruby
begin
  # Delete an item category
  data, status_code, headers = api_instance.delete_item_category_async_with_http_info(tenant_id, item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->delete_item_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_categories_async

> <ItemCategoryDtoListEnvelope> get_item_categories_async(opts)

Get all item categories

Retrieves all item categories for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_category_dto_collection_query_parameters: OpenapiClient::ItemCategoryDtoCollectionQueryParameters.new # ItemCategoryDtoCollectionQueryParameters | 
}

begin
  # Get all item categories
  result = api_instance.get_item_categories_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->get_item_categories_async: #{e}"
end
```

#### Using the get_item_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoListEnvelope>, Integer, Hash)> get_item_categories_async_with_http_info(opts)

```ruby
begin
  # Get all item categories
  data, status_code, headers = api_instance.get_item_categories_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->get_item_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_category_dto_collection_query_parameters** | [**ItemCategoryDtoCollectionQueryParameters**](ItemCategoryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemCategoryDtoListEnvelope**](ItemCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_category_by_id_async

> <ItemCategoryDtoEnvelope> get_item_category_by_id_async(item_category_id, opts)

Get item category by ID

Retrieves a specific item category by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item category by ID
  result = api_instance.get_item_category_by_id_async(item_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->get_item_category_by_id_async: #{e}"
end
```

#### Using the get_item_category_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCategoryDtoEnvelope>, Integer, Hash)> get_item_category_by_id_async_with_http_info(item_category_id, opts)

```ruby
begin
  # Get item category by ID
  data, status_code, headers = api_instance.get_item_category_by_id_async_with_http_info(item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->get_item_category_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_category_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemCategoryDtoEnvelope**](ItemCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_item_category_async

> patch_item_category_async(tenant_id, item_category_id, opts)

Patch an item category

Partially updates an existing item category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an item category
  api_instance.patch_item_category_async(tenant_id, item_category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->patch_item_category_async: #{e}"
end
```

#### Using the patch_item_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_item_category_async_with_http_info(tenant_id, item_category_id, opts)

```ruby
begin
  # Patch an item category
  data, status_code, headers = api_instance.patch_item_category_async_with_http_info(tenant_id, item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->patch_item_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_category_async

> update_item_category_async(tenant_id, item_category_id, opts)

Update an item category

Updates an existing item category for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_category_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_category_update_dto: OpenapiClient::ItemCategoryUpdateDto.new({title: 'title_example'}) # ItemCategoryUpdateDto | 
}

begin
  # Update an item category
  api_instance.update_item_category_async(tenant_id, item_category_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->update_item_category_async: #{e}"
end
```

#### Using the update_item_category_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_category_async_with_http_info(tenant_id, item_category_id, opts)

```ruby
begin
  # Update an item category
  data, status_code, headers = api_instance.update_item_category_async_with_http_info(tenant_id, item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemCategoriesApi->update_item_category_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_category_update_dto** | [**ItemCategoryUpdateDto**](ItemCategoryUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

