# OpenapiClient::ItemGoogleCategoriesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_all_item_google_categories_async**](ItemGoogleCategoriesApi.md#get_all_item_google_categories_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/All | Get all Google item categories (all) |
| [**get_children_item_google_categories_by_id_async**](ItemGoogleCategoriesApi.md#get_children_item_google_categories_by_id_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/{itemCategoryId}/Children | Get children Google item categories by ID |
| [**get_item_google_categories_async**](ItemGoogleCategoriesApi.md#get_item_google_categories_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories | Get all Google item categories |
| [**get_item_google_categories_count_async**](ItemGoogleCategoriesApi.md#get_item_google_categories_count_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/Count | Get Google item categories count |
| [**get_item_google_categories_tree_async**](ItemGoogleCategoriesApi.md#get_item_google_categories_tree_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/tree | Get Google item categories tree |
| [**get_item_google_category_by_id_async**](ItemGoogleCategoriesApi.md#get_item_google_category_by_id_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/{itemCategoryId} | Get Google item category by ID |
| [**get_root_item_google_categories_async**](ItemGoogleCategoriesApi.md#get_root_item_google_categories_async) | **GET** /api/v2/CatalogService/ItemGoogleCategories/Primary | Get root Google item categories |
| [**map_item_google_categories_tree_async**](ItemGoogleCategoriesApi.md#map_item_google_categories_tree_async) | **POST** /api/v2/CatalogService/ItemGoogleCategories/tree | Map Google item categories tree |


## get_all_item_google_categories_async

> <ItemGoogleCategoryDtoListEnvelope> get_all_item_google_categories_async(opts)

Get all Google item categories (all)

Retrieves all Google item categories (all) without OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all Google item categories (all)
  result = api_instance.get_all_item_google_categories_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_all_item_google_categories_async: #{e}"
end
```

#### Using the get_all_item_google_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> get_all_item_google_categories_async_with_http_info(opts)

```ruby
begin
  # Get all Google item categories (all)
  data, status_code, headers = api_instance.get_all_item_google_categories_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_all_item_google_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_children_item_google_categories_by_id_async

> <ItemGoogleCategoryDtoListEnvelope> get_children_item_google_categories_by_id_async(item_category_id, opts)

Get children Google item categories by ID

Retrieves children Google item categories for a given ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
item_category_id = 'item_category_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get children Google item categories by ID
  result = api_instance.get_children_item_google_categories_by_id_async(item_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_children_item_google_categories_by_id_async: #{e}"
end
```

#### Using the get_children_item_google_categories_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> get_children_item_google_categories_by_id_async_with_http_info(item_category_id, opts)

```ruby
begin
  # Get children Google item categories by ID
  data, status_code, headers = api_instance.get_children_item_google_categories_by_id_async_with_http_info(item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_children_item_google_categories_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_google_categories_async

> <ItemGoogleCategoryDtoListEnvelope> get_item_google_categories_async(opts)

Get all Google item categories

Retrieves all Google item categories using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all Google item categories
  result = api_instance.get_item_google_categories_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_categories_async: #{e}"
end
```

#### Using the get_item_google_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> get_item_google_categories_async_with_http_info(opts)

```ruby
begin
  # Get all Google item categories
  data, status_code, headers = api_instance.get_item_google_categories_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_google_categories_count_async

> <Int32Envelope> get_item_google_categories_count_async(opts)

Get Google item categories count

Retrieves the count of Google item categories using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Google item categories count
  result = api_instance.get_item_google_categories_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_categories_count_async: #{e}"
end
```

#### Using the get_item_google_categories_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_google_categories_count_async_with_http_info(opts)

```ruby
begin
  # Get Google item categories count
  data, status_code, headers = api_instance.get_item_google_categories_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_categories_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_google_categories_tree_async

> <ItemGoogleCategoryDtoListEnvelope> get_item_google_categories_tree_async(opts)

Get Google item categories tree

Retrieves the Google item categories tree.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Google item categories tree
  result = api_instance.get_item_google_categories_tree_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_categories_tree_async: #{e}"
end
```

#### Using the get_item_google_categories_tree_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> get_item_google_categories_tree_async_with_http_info(opts)

```ruby
begin
  # Get Google item categories tree
  data, status_code, headers = api_instance.get_item_google_categories_tree_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_categories_tree_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_google_category_by_id_async

> <ItemGoogleCategoryDtoEnvelope> get_item_google_category_by_id_async(item_category_id, opts)

Get Google item category by ID

Retrieves a specific Google item category by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
item_category_id = 'item_category_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get Google item category by ID
  result = api_instance.get_item_google_category_by_id_async(item_category_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_category_by_id_async: #{e}"
end
```

#### Using the get_item_google_category_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoEnvelope>, Integer, Hash)> get_item_google_category_by_id_async_with_http_info(item_category_id, opts)

```ruby
begin
  # Get Google item category by ID
  data, status_code, headers = api_instance.get_item_google_category_by_id_async_with_http_info(item_category_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_item_google_category_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_category_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoEnvelope**](ItemGoogleCategoryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_root_item_google_categories_async

> <ItemGoogleCategoryDtoListEnvelope> get_root_item_google_categories_async(opts)

Get root Google item categories

Retrieves root Google item categories.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get root Google item categories
  result = api_instance.get_root_item_google_categories_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_root_item_google_categories_async: #{e}"
end
```

#### Using the get_root_item_google_categories_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> get_root_item_google_categories_async_with_http_info(opts)

```ruby
begin
  # Get root Google item categories
  data, status_code, headers = api_instance.get_root_item_google_categories_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->get_root_item_google_categories_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## map_item_google_categories_tree_async

> <ItemGoogleCategoryDtoListEnvelope> map_item_google_categories_tree_async(tenant_id, opts)

Map Google item categories tree

Maps the Google item categories tree.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemGoogleCategoriesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Map Google item categories tree
  result = api_instance.map_item_google_categories_tree_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->map_item_google_categories_tree_async: #{e}"
end
```

#### Using the map_item_google_categories_tree_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemGoogleCategoryDtoListEnvelope>, Integer, Hash)> map_item_google_categories_tree_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Map Google item categories tree
  data, status_code, headers = api_instance.map_item_google_categories_tree_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemGoogleCategoryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemGoogleCategoriesApi->map_item_google_categories_tree_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemGoogleCategoryDtoListEnvelope**](ItemGoogleCategoryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

