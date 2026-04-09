# OpenapiClient::ItemAttachmentsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_attachment_async**](ItemAttachmentsApi.md#create_item_attachment_async) | **POST** /api/v2/CatalogService/ItemAttachments | Create a new item attachment |
| [**delete_item_attachment_async**](ItemAttachmentsApi.md#delete_item_attachment_async) | **DELETE** /api/v2/CatalogService/ItemAttachments/{itemAttachmentId} | Delete an item attachment |
| [**get_item_attachment_by_id_async**](ItemAttachmentsApi.md#get_item_attachment_by_id_async) | **GET** /api/v2/CatalogService/ItemAttachments/{itemAttachmentId} | Get item attachment by ID |
| [**get_item_attachments_async**](ItemAttachmentsApi.md#get_item_attachments_async) | **GET** /api/v2/CatalogService/ItemAttachments | Get all item attachments |
| [**update_item_attachment_async**](ItemAttachmentsApi.md#update_item_attachment_async) | **PUT** /api/v2/CatalogService/ItemAttachments/{itemAttachmentId} | Update an item attachment |


## create_item_attachment_async

> <ItemAttachmentDtoEnvelope> create_item_attachment_async(tenant_id, opts)

Create a new item attachment

Creates a new item attachment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attachment_create_dto: OpenapiClient::ItemAttachmentCreateDto.new # ItemAttachmentCreateDto | 
}

begin
  # Create a new item attachment
  result = api_instance.create_item_attachment_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->create_item_attachment_async: #{e}"
end
```

#### Using the create_item_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoEnvelope>, Integer, Hash)> create_item_attachment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item attachment
  data, status_code, headers = api_instance.create_item_attachment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->create_item_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attachment_create_dto** | [**ItemAttachmentCreateDto**](ItemAttachmentCreateDto.md) |  | [optional] |

### Return type

[**ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_attachment_async

> <EmptyEnvelope> delete_item_attachment_async(tenant_id, item_attachment_id, opts)

Delete an item attachment

Deletes an item attachment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item attachment
  result = api_instance.delete_item_attachment_async(tenant_id, item_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->delete_item_attachment_async: #{e}"
end
```

#### Using the delete_item_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_attachment_async_with_http_info(tenant_id, item_attachment_id, opts)

```ruby
begin
  # Delete an item attachment
  data, status_code, headers = api_instance.delete_item_attachment_async_with_http_info(tenant_id, item_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->delete_item_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attachment_by_id_async

> <ItemAttachmentDtoEnvelope> get_item_attachment_by_id_async(item_attachment_id, opts)

Get item attachment by ID

Retrieves a specific item attachment by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttachmentsApi.new
item_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item attachment by ID
  result = api_instance.get_item_attachment_by_id_async(item_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->get_item_attachment_by_id_async: #{e}"
end
```

#### Using the get_item_attachment_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoEnvelope>, Integer, Hash)> get_item_attachment_by_id_async_with_http_info(item_attachment_id, opts)

```ruby
begin
  # Get item attachment by ID
  data, status_code, headers = api_instance.get_item_attachment_by_id_async_with_http_info(item_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->get_item_attachment_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttachmentDtoEnvelope**](ItemAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attachments_async

> <ItemAttachmentDtoListEnvelope> get_item_attachments_async(tenant_id, opts)

Get all item attachments

Retrieves all item attachments for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item attachments
  result = api_instance.get_item_attachments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->get_item_attachments_async: #{e}"
end
```

#### Using the get_item_attachments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttachmentDtoListEnvelope>, Integer, Hash)> get_item_attachments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item attachments
  data, status_code, headers = api_instance.get_item_attachments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttachmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->get_item_attachments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttachmentDtoListEnvelope**](ItemAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_attachment_async

> <EmptyEnvelope> update_item_attachment_async(tenant_id, item_attachment_id, opts)

Update an item attachment

Updates an existing item attachment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attachment_update_dto: OpenapiClient::ItemAttachmentUpdateDto.new # ItemAttachmentUpdateDto | 
}

begin
  # Update an item attachment
  result = api_instance.update_item_attachment_async(tenant_id, item_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->update_item_attachment_async: #{e}"
end
```

#### Using the update_item_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_attachment_async_with_http_info(tenant_id, item_attachment_id, opts)

```ruby
begin
  # Update an item attachment
  data, status_code, headers = api_instance.update_item_attachment_async_with_http_info(tenant_id, item_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttachmentsApi->update_item_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attachment_update_dto** | [**ItemAttachmentUpdateDto**](ItemAttachmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

