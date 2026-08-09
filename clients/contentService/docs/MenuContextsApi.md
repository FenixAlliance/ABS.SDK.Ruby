# OpenapiClient::MenuContextsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_menu_contexts_async**](MenuContextsApi.md#count_menu_contexts_async) | **GET** /api/v2/ContentService/MenuContexts/Count | Count menu contexts |
| [**create_menu_context_async**](MenuContextsApi.md#create_menu_context_async) | **POST** /api/v2/ContentService/MenuContexts | Create a menu context |
| [**delete_menu_context_async**](MenuContextsApi.md#delete_menu_context_async) | **DELETE** /api/v2/ContentService/MenuContexts/{menuContextId} | Delete a menu context |
| [**get_menu_context_by_id_async**](MenuContextsApi.md#get_menu_context_by_id_async) | **GET** /api/v2/ContentService/MenuContexts/{menuContextId} | Get menu context by ID |
| [**get_menu_contexts_async**](MenuContextsApi.md#get_menu_contexts_async) | **GET** /api/v2/ContentService/MenuContexts | Get menu contexts |
| [**update_menu_context_async**](MenuContextsApi.md#update_menu_context_async) | **PUT** /api/v2/ContentService/MenuContexts/{menuContextId} | Update a menu context |


## count_menu_contexts_async

> <Int32Envelope> count_menu_contexts_async(tenant_id, opts)

Count menu contexts

Counts all menu contexts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MenuContextsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  menu_context_dto_collection_query_parameters: OpenapiClient::MenuContextDtoCollectionQueryParameters.new # MenuContextDtoCollectionQueryParameters | 
}

begin
  # Count menu contexts
  result = api_instance.count_menu_contexts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->count_menu_contexts_async: #{e}"
end
```

#### Using the count_menu_contexts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_menu_contexts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count menu contexts
  data, status_code, headers = api_instance.count_menu_contexts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->count_menu_contexts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **menu_context_dto_collection_query_parameters** | [**MenuContextDtoCollectionQueryParameters**](MenuContextDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_menu_context_async

> <EmptyEnvelope> create_menu_context_async(tenant_id, menu_context_create_dto, opts)

Create a menu context

Creates a new menu context for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MenuContextsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
menu_context_create_dto = OpenapiClient::MenuContextCreateDto.new({name: 'name_example'}) # MenuContextCreateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Create a menu context
  result = api_instance.create_menu_context_async(tenant_id, menu_context_create_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->create_menu_context_async: #{e}"
end
```

#### Using the create_menu_context_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_menu_context_async_with_http_info(tenant_id, menu_context_create_dto, opts)

```ruby
begin
  # Create a menu context
  data, status_code, headers = api_instance.create_menu_context_async_with_http_info(tenant_id, menu_context_create_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->create_menu_context_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **menu_context_create_dto** | [**MenuContextCreateDto**](MenuContextCreateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_menu_context_async

> <EmptyEnvelope> delete_menu_context_async(tenant_id, menu_context_id, opts)

Delete a menu context

Deletes a menu context for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MenuContextsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
menu_context_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a menu context
  result = api_instance.delete_menu_context_async(tenant_id, menu_context_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->delete_menu_context_async: #{e}"
end
```

#### Using the delete_menu_context_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_menu_context_async_with_http_info(tenant_id, menu_context_id, opts)

```ruby
begin
  # Delete a menu context
  data, status_code, headers = api_instance.delete_menu_context_async_with_http_info(tenant_id, menu_context_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->delete_menu_context_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **menu_context_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_menu_context_by_id_async

> <MenuContextDtoEnvelope> get_menu_context_by_id_async(tenant_id, menu_context_id, opts)

Get menu context by ID

Retrieves a specific menu context by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MenuContextsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
menu_context_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get menu context by ID
  result = api_instance.get_menu_context_by_id_async(tenant_id, menu_context_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->get_menu_context_by_id_async: #{e}"
end
```

#### Using the get_menu_context_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MenuContextDtoEnvelope>, Integer, Hash)> get_menu_context_by_id_async_with_http_info(tenant_id, menu_context_id, opts)

```ruby
begin
  # Get menu context by ID
  data, status_code, headers = api_instance.get_menu_context_by_id_async_with_http_info(tenant_id, menu_context_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MenuContextDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->get_menu_context_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **menu_context_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**MenuContextDtoEnvelope**](MenuContextDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_menu_contexts_async

> <MenuContextDtoListEnvelope> get_menu_contexts_async(tenant_id, opts)

Get menu contexts

Retrieves all menu contexts for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MenuContextsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  menu_context_dto_collection_query_parameters: OpenapiClient::MenuContextDtoCollectionQueryParameters.new # MenuContextDtoCollectionQueryParameters | 
}

begin
  # Get menu contexts
  result = api_instance.get_menu_contexts_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->get_menu_contexts_async: #{e}"
end
```

#### Using the get_menu_contexts_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MenuContextDtoListEnvelope>, Integer, Hash)> get_menu_contexts_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get menu contexts
  data, status_code, headers = api_instance.get_menu_contexts_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MenuContextDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->get_menu_contexts_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **menu_context_dto_collection_query_parameters** | [**MenuContextDtoCollectionQueryParameters**](MenuContextDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**MenuContextDtoListEnvelope**](MenuContextDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_menu_context_async

> <EmptyEnvelope> update_menu_context_async(tenant_id, menu_context_id, menu_context_update_dto, opts)

Update a menu context

Updates an existing menu context for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MenuContextsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
menu_context_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
menu_context_update_dto = OpenapiClient::MenuContextUpdateDto.new # MenuContextUpdateDto | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update a menu context
  result = api_instance.update_menu_context_async(tenant_id, menu_context_id, menu_context_update_dto, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->update_menu_context_async: #{e}"
end
```

#### Using the update_menu_context_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_menu_context_async_with_http_info(tenant_id, menu_context_id, menu_context_update_dto, opts)

```ruby
begin
  # Update a menu context
  data, status_code, headers = api_instance.update_menu_context_async_with_http_info(tenant_id, menu_context_id, menu_context_update_dto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MenuContextsApi->update_menu_context_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **menu_context_id** | **String** |  |  |
| **menu_context_update_dto** | [**MenuContextUpdateDto**](MenuContextUpdateDto.md) |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

