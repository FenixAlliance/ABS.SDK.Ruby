# OpenapiClient::ItemAttributeOptionsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_attribute_option_async**](ItemAttributeOptionsApi.md#create_item_attribute_option_async) | **POST** /api/v2/CatalogService/ItemAttributeOptions | Create a new item attribute option |
| [**delete_item_attribute_option_async**](ItemAttributeOptionsApi.md#delete_item_attribute_option_async) | **DELETE** /api/v2/CatalogService/ItemAttributeOptions/{itemAttributeOptionId} | Delete an item attribute option |
| [**get_item_attribute_option_by_id_async**](ItemAttributeOptionsApi.md#get_item_attribute_option_by_id_async) | **GET** /api/v2/CatalogService/ItemAttributeOptions/{itemAttributeOptionId} | Get item attribute option by ID |
| [**get_item_attribute_options_async**](ItemAttributeOptionsApi.md#get_item_attribute_options_async) | **GET** /api/v2/CatalogService/ItemAttributeOptions | Get all item attribute options |
| [**get_item_attribute_options_count_async**](ItemAttributeOptionsApi.md#get_item_attribute_options_count_async) | **GET** /api/v2/CatalogService/ItemAttributeOptions/Count | Get item attribute options count |
| [**update_item_attribute_option_async**](ItemAttributeOptionsApi.md#update_item_attribute_option_async) | **PUT** /api/v2/CatalogService/ItemAttributeOptions/{itemAttributeOptionId} | Update an item attribute option |


## create_item_attribute_option_async

> <ItemAttributeOptionDtoEnvelope> create_item_attribute_option_async(tenant_id, opts)

Create a new item attribute option

Creates a new item attribute option for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributeOptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attribute_option_create_dto: OpenapiClient::ItemAttributeOptionCreateDto.new({name: 'name_example', item_attribute_id: 'item_attribute_id_example'}) # ItemAttributeOptionCreateDto | 
}

begin
  # Create a new item attribute option
  result = api_instance.create_item_attribute_option_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->create_item_attribute_option_async: #{e}"
end
```

#### Using the create_item_attribute_option_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoEnvelope>, Integer, Hash)> create_item_attribute_option_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new item attribute option
  data, status_code, headers = api_instance.create_item_attribute_option_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->create_item_attribute_option_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attribute_option_create_dto** | [**ItemAttributeOptionCreateDto**](ItemAttributeOptionCreateDto.md) |  | [optional] |

### Return type

[**ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_attribute_option_async

> delete_item_attribute_option_async(tenant_id, item_attribute_option_id, opts)

Delete an item attribute option

Deletes an item attribute option for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributeOptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item attribute option
  api_instance.delete_item_attribute_option_async(tenant_id, item_attribute_option_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->delete_item_attribute_option_async: #{e}"
end
```

#### Using the delete_item_attribute_option_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_item_attribute_option_async_with_http_info(tenant_id, item_attribute_option_id, opts)

```ruby
begin
  # Delete an item attribute option
  data, status_code, headers = api_instance.delete_item_attribute_option_async_with_http_info(tenant_id, item_attribute_option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->delete_item_attribute_option_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attribute_option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attribute_option_by_id_async

> <ItemAttributeOptionDtoEnvelope> get_item_attribute_option_by_id_async(item_attribute_option_id, opts)

Get item attribute option by ID

Retrieves a specific item attribute option by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributeOptionsApi.new
item_attribute_option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item attribute option by ID
  result = api_instance.get_item_attribute_option_by_id_async(item_attribute_option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->get_item_attribute_option_by_id_async: #{e}"
end
```

#### Using the get_item_attribute_option_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoEnvelope>, Integer, Hash)> get_item_attribute_option_by_id_async_with_http_info(item_attribute_option_id, opts)

```ruby
begin
  # Get item attribute option by ID
  data, status_code, headers = api_instance.get_item_attribute_option_by_id_async_with_http_info(item_attribute_option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->get_item_attribute_option_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **item_attribute_option_id** | **String** |  |  |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attribute_options_async

> <ItemAttributeOptionDtoListEnvelope> get_item_attribute_options_async(opts)

Get all item attribute options

Retrieves all item attribute options for the specified tenant using OData query options.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributeOptionsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item attribute options
  result = api_instance.get_item_attribute_options_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->get_item_attribute_options_async: #{e}"
end
```

#### Using the get_item_attribute_options_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoListEnvelope>, Integer, Hash)> get_item_attribute_options_async_with_http_info(opts)

```ruby
begin
  # Get all item attribute options
  data, status_code, headers = api_instance.get_item_attribute_options_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->get_item_attribute_options_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemAttributeOptionDtoListEnvelope**](ItemAttributeOptionDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_attribute_options_count_async

> <Int32Envelope> get_item_attribute_options_count_async(opts)

Get item attribute options count

Returns the count of item attribute options for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributeOptionsApi.new
opts = {
  tenant_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item attribute options count
  result = api_instance.get_item_attribute_options_count_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->get_item_attribute_options_count_async: #{e}"
end
```

#### Using the get_item_attribute_options_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_attribute_options_count_async_with_http_info(opts)

```ruby
begin
  # Get item attribute options count
  data, status_code, headers = api_instance.get_item_attribute_options_count_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->get_item_attribute_options_count_async_with_http_info: #{e}"
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


## update_item_attribute_option_async

> <ItemAttributeOptionDtoEnvelope> update_item_attribute_option_async(tenant_id, item_attribute_option_id, opts)

Update an item attribute option

Updates an existing item attribute option for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemAttributeOptionsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
item_attribute_option_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_attribute_option_update_dto: OpenapiClient::ItemAttributeOptionUpdateDto.new({name: 'name_example'}) # ItemAttributeOptionUpdateDto | 
}

begin
  # Update an item attribute option
  result = api_instance.update_item_attribute_option_async(tenant_id, item_attribute_option_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->update_item_attribute_option_async: #{e}"
end
```

#### Using the update_item_attribute_option_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemAttributeOptionDtoEnvelope>, Integer, Hash)> update_item_attribute_option_async_with_http_info(tenant_id, item_attribute_option_id, opts)

```ruby
begin
  # Update an item attribute option
  data, status_code, headers = api_instance.update_item_attribute_option_async_with_http_info(tenant_id, item_attribute_option_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemAttributeOptionDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemAttributeOptionsApi->update_item_attribute_option_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **item_attribute_option_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_attribute_option_update_dto** | [**ItemAttributeOptionUpdateDto**](ItemAttributeOptionUpdateDto.md) |  | [optional] |

### Return type

[**ItemAttributeOptionDtoEnvelope**](ItemAttributeOptionDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

