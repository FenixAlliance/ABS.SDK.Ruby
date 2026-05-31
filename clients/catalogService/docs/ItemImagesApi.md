# OpenapiClient::ItemImagesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_image_async**](ItemImagesApi.md#create_item_image_async) | **POST** /api/v2/CatalogService/ItemImages | Create a new item image |
| [**delete_item_image_async**](ItemImagesApi.md#delete_item_image_async) | **DELETE** /api/v2/CatalogService/ItemImages/{itemImageId} | Delete an item image |
| [**get_item_image_by_id_async**](ItemImagesApi.md#get_item_image_by_id_async) | **GET** /api/v2/CatalogService/ItemImages/{itemImageId} | Get item image by ID |
| [**get_item_images_async**](ItemImagesApi.md#get_item_images_async) | **GET** /api/v2/CatalogService/ItemImages | Get all item images |
| [**update_item_image_async**](ItemImagesApi.md#update_item_image_async) | **PUT** /api/v2/CatalogService/ItemImages/{itemImageId} | Update an item image |


## create_item_image_async

> <ItemImageDtoEnvelope> create_item_image_async(tenant_id, opts)

Create a new item image

Creates a new item image for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemImagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_image_create_dto: OpenapiClient::ItemImageCreateDto.new({file_name: 'file_name_example'}) # ItemImageCreateDto | 
}

begin
  # Create a new item image
  result = api_instance.create_item_image_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->create_item_image_async: #{e}"
end
```

#### Using the create_item_image_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoEnvelope>, Integer, Hash)> create_item_image_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item image
  data, status_code, headers = api_instance.create_item_image_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->create_item_image_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_image_create_dto** | [**ItemImageCreateDto**](ItemImageCreateDto.md) |  | [optional] |

### Return type

[**ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_image_async

> delete_item_image_async(tenant_id, item_image_id, opts)

Delete an item image

Deletes an item image for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemImagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_image_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item image
  api_instance.delete_item_image_async(tenant_id, item_image_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->delete_item_image_async: #{e}"
end
```

#### Using the delete_item_image_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_image_async_with_http_info(tenant_id, item_image_id, opts)

```ruby
begin
  # Delete an item image
  data, status_code, headers = api_instance.delete_item_image_async_with_http_info(tenant_id, item_image_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->delete_item_image_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_image_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_image_by_id_async

> <ItemImageDtoEnvelope> get_item_image_by_id_async(item_image_id, opts)

Get item image by ID

Retrieves a specific item image by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemImagesApi.new
item_image_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item image by ID
  result = api_instance.get_item_image_by_id_async(item_image_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->get_item_image_by_id_async: #{e}"
end
```

#### Using the get_item_image_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoEnvelope>, Integer, Hash)> get_item_image_by_id_async_with_http_info(item_image_id, opts)

```ruby
begin
  # Get item image by ID
  data, status_code, headers = api_instance.get_item_image_by_id_async_with_http_info(item_image_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->get_item_image_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_image_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemImageDtoEnvelope**](ItemImageDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_images_async

> <ItemImageDtoListEnvelope> get_item_images_async(opts)

Get all item images

Retrieves all item images for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemImagesApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item images
  result = api_instance.get_item_images_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->get_item_images_async: #{e}"
end
```

#### Using the get_item_images_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemImageDtoListEnvelope>, Integer, Hash)> get_item_images_async_with_http_info(opts)

```ruby
begin
  # Get all item images
  data, status_code, headers = api_instance.get_item_images_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemImageDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->get_item_images_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemImageDtoListEnvelope**](ItemImageDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_image_async

> update_item_image_async(tenant_id, item_image_id, opts)

Update an item image

Updates an existing item image for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemImagesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_image_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_image_update_dto: OpenapiClient::ItemImageUpdateDto.new({item_id: 'item_id_example', m_d5_hash: 'm_d5_hash_example', file_upload_url: 'file_upload_url_example', file_name: 'file_name_example', content_type: 'content_type_example'}) # ItemImageUpdateDto | 
}

begin
  # Update an item image
  api_instance.update_item_image_async(tenant_id, item_image_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->update_item_image_async: #{e}"
end
```

#### Using the update_item_image_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_image_async_with_http_info(tenant_id, item_image_id, opts)

```ruby
begin
  # Update an item image
  data, status_code, headers = api_instance.update_item_image_async_with_http_info(tenant_id, item_image_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemImagesApi->update_item_image_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_image_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_image_update_dto** | [**ItemImageUpdateDto**](ItemImageUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

