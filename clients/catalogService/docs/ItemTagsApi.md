# OpenapiClient::ItemTagsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_tag_async**](ItemTagsApi.md#create_item_tag_async) | **POST** /api/v2/CatalogService/ItemTags | Create a new item tag |
| [**delete_item_tag_async**](ItemTagsApi.md#delete_item_tag_async) | **DELETE** /api/v2/CatalogService/ItemTags/{itemTagId} | Delete an item tag |
| [**get_item_tag_by_id_async**](ItemTagsApi.md#get_item_tag_by_id_async) | **GET** /api/v2/CatalogService/ItemTags/{itemTagId} | Get item tag by ID |
| [**get_item_tags_async**](ItemTagsApi.md#get_item_tags_async) | **GET** /api/v2/CatalogService/ItemTags | Get all item tags |
| [**patch_item_tag_async**](ItemTagsApi.md#patch_item_tag_async) | **PATCH** /api/v2/CatalogService/ItemTags/{itemTagId} | Patch an item tag |
| [**update_item_tag_async**](ItemTagsApi.md#update_item_tag_async) | **PUT** /api/v2/CatalogService/ItemTags/{itemTagId} | Update an item tag |


## create_item_tag_async

> <ItemTagDtoEnvelope> create_item_tag_async(tenant_id, opts)

Create a new item tag

Creates a new item tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_tag_create_dto: OpenapiClient::ItemTagCreateDto.new({title: 'title_example'}) # ItemTagCreateDto | 
}

begin
  # Create a new item tag
  result = api_instance.create_item_tag_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->create_item_tag_async: #{e}"
end
```

#### Using the create_item_tag_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoEnvelope>, Integer, Hash)> create_item_tag_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item tag
  data, status_code, headers = api_instance.create_item_tag_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->create_item_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_tag_create_dto** | [**ItemTagCreateDto**](ItemTagCreateDto.md) |  | [optional] |

### Return type

[**ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_tag_async

> delete_item_tag_async(tenant_id, item_tag_id, opts)

Delete an item tag

Deletes an item tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item tag
  api_instance.delete_item_tag_async(tenant_id, item_tag_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->delete_item_tag_async: #{e}"
end
```

#### Using the delete_item_tag_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_tag_async_with_http_info(tenant_id, item_tag_id, opts)

```ruby
begin
  # Delete an item tag
  data, status_code, headers = api_instance.delete_item_tag_async_with_http_info(tenant_id, item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->delete_item_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_tag_by_id_async

> <ItemTagDtoEnvelope> get_item_tag_by_id_async(item_tag_id, opts)

Get item tag by ID

Retrieves a specific item tag by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTagsApi.new
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item tag by ID
  result = api_instance.get_item_tag_by_id_async(item_tag_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->get_item_tag_by_id_async: #{e}"
end
```

#### Using the get_item_tag_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoEnvelope>, Integer, Hash)> get_item_tag_by_id_async_with_http_info(item_tag_id, opts)

```ruby
begin
  # Get item tag by ID
  data, status_code, headers = api_instance.get_item_tag_by_id_async_with_http_info(item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->get_item_tag_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_tag_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTagDtoEnvelope**](ItemTagDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_tags_async

> <ItemTagDtoListEnvelope> get_item_tags_async(opts)

Get all item tags

Retrieves all item tags for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTagsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item tags
  result = api_instance.get_item_tags_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->get_item_tags_async: #{e}"
end
```

#### Using the get_item_tags_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemTagDtoListEnvelope>, Integer, Hash)> get_item_tags_async_with_http_info(opts)

```ruby
begin
  # Get all item tags
  data, status_code, headers = api_instance.get_item_tags_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemTagDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->get_item_tags_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemTagDtoListEnvelope**](ItemTagDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_item_tag_async

> patch_item_tag_async(tenant_id, item_tag_id, opts)

Patch an item tag

Partially updates an existing item tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch an item tag
  api_instance.patch_item_tag_async(tenant_id, item_tag_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->patch_item_tag_async: #{e}"
end
```

#### Using the patch_item_tag_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> patch_item_tag_async_with_http_info(tenant_id, item_tag_id, opts)

```ruby
begin
  # Patch an item tag
  data, status_code, headers = api_instance.patch_item_tag_async_with_http_info(tenant_id, item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->patch_item_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_tag_id** | **String** |  |  |
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


## update_item_tag_async

> update_item_tag_async(tenant_id, item_tag_id, opts)

Update an item tag

Updates an existing item tag for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemTagsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_tag_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_tag_update_dto: OpenapiClient::ItemTagUpdateDto.new({title: 'title_example'}) # ItemTagUpdateDto | 
}

begin
  # Update an item tag
  api_instance.update_item_tag_async(tenant_id, item_tag_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->update_item_tag_async: #{e}"
end
```

#### Using the update_item_tag_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_item_tag_async_with_http_info(tenant_id, item_tag_id, opts)

```ruby
begin
  # Update an item tag
  data, status_code, headers = api_instance.update_item_tag_async_with_http_info(tenant_id, item_tag_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemTagsApi->update_item_tag_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_tag_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_tag_update_dto** | [**ItemTagUpdateDto**](ItemTagUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

