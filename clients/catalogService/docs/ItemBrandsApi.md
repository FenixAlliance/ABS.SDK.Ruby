# OpenapiClient::ItemBrandsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_brand_async**](ItemBrandsApi.md#create_item_brand_async) | **POST** /api/v2/CatalogService/ItemBrands | Create a new item brand |
| [**delete_item_brand_async**](ItemBrandsApi.md#delete_item_brand_async) | **DELETE** /api/v2/CatalogService/ItemBrands/{itemBrandId} | Delete an item brand |
| [**get_item_brand_by_id_async**](ItemBrandsApi.md#get_item_brand_by_id_async) | **GET** /api/v2/CatalogService/ItemBrands/{itemBrandId} | Get item brand by ID |
| [**get_item_brands_async**](ItemBrandsApi.md#get_item_brands_async) | **GET** /api/v2/CatalogService/ItemBrands | Get all item brands |
| [**update_item_brand_async**](ItemBrandsApi.md#update_item_brand_async) | **PUT** /api/v2/CatalogService/ItemBrands/{itemBrandId} | Update an item brand |


## create_item_brand_async

> <ItemBrandDtoEnvelope> create_item_brand_async(tenant_id, opts)

Create a new item brand

Creates a new item brand for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBrandsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_brand_create_dto: OpenapiClient::ItemBrandCreateDto.new({name: 'name_example', business_id: 'business_id_example'}) # ItemBrandCreateDto | 
}

begin
  # Create a new item brand
  result = api_instance.create_item_brand_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->create_item_brand_async: #{e}"
end
```

#### Using the create_item_brand_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoEnvelope>, Integer, Hash)> create_item_brand_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item brand
  data, status_code, headers = api_instance.create_item_brand_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->create_item_brand_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_brand_create_dto** | [**ItemBrandCreateDto**](ItemBrandCreateDto.md) |  | [optional] |

### Return type

[**ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_brand_async

> delete_item_brand_async(tenant_id, item_brand_id, opts)

Delete an item brand

Deletes an item brand for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBrandsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_brand_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item brand
  api_instance.delete_item_brand_async(tenant_id, item_brand_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->delete_item_brand_async: #{e}"
end
```

#### Using the delete_item_brand_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_brand_async_with_http_info(tenant_id, item_brand_id, opts)

```ruby
begin
  # Delete an item brand
  data, status_code, headers = api_instance.delete_item_brand_async_with_http_info(tenant_id, item_brand_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->delete_item_brand_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_brand_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_brand_by_id_async

> <ItemBrandDtoEnvelope> get_item_brand_by_id_async(item_brand_id, opts)

Get item brand by ID

Retrieves a specific item brand by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBrandsApi.new
item_brand_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item brand by ID
  result = api_instance.get_item_brand_by_id_async(item_brand_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->get_item_brand_by_id_async: #{e}"
end
```

#### Using the get_item_brand_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoEnvelope>, Integer, Hash)> get_item_brand_by_id_async_with_http_info(item_brand_id, opts)

```ruby
begin
  # Get item brand by ID
  data, status_code, headers = api_instance.get_item_brand_by_id_async_with_http_info(item_brand_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->get_item_brand_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_brand_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_brands_async

> <ItemBrandDtoListEnvelope> get_item_brands_async(tenant_id, opts)

Get all item brands

Retrieves all item brands for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBrandsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item brands
  result = api_instance.get_item_brands_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->get_item_brands_async: #{e}"
end
```

#### Using the get_item_brands_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoListEnvelope>, Integer, Hash)> get_item_brands_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item brands
  data, status_code, headers = api_instance.get_item_brands_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->get_item_brands_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemBrandDtoListEnvelope**](ItemBrandDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_brand_async

> <ItemBrandDtoEnvelope> update_item_brand_async(tenant_id, item_brand_id, opts)

Update an item brand

Updates an existing item brand for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemBrandsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_brand_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_brand_update_dto: OpenapiClient::ItemBrandUpdateDto.new({name: 'name_example'}) # ItemBrandUpdateDto | 
}

begin
  # Update an item brand
  result = api_instance.update_item_brand_async(tenant_id, item_brand_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->update_item_brand_async: #{e}"
end
```

#### Using the update_item_brand_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemBrandDtoEnvelope>, Integer, Hash)> update_item_brand_async_with_http_info(tenant_id, item_brand_id, opts)

```ruby
begin
  # Update an item brand
  data, status_code, headers = api_instance.update_item_brand_async_with_http_info(tenant_id, item_brand_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemBrandDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemBrandsApi->update_item_brand_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_brand_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_brand_update_dto** | [**ItemBrandUpdateDto**](ItemBrandUpdateDto.md) |  | [optional] |

### Return type

[**ItemBrandDtoEnvelope**](ItemBrandDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

