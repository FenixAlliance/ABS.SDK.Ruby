# OpenapiClient::ItemPickListsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_pick_list_async**](ItemPickListsApi.md#create_item_pick_list_async) | **POST** /api/v2/LogisticsService/ItemPickLists | Create an item pick list |
| [**create_item_pick_list_entry_async**](ItemPickListsApi.md#create_item_pick_list_entry_async) | **POST** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Create a pick list entry |
| [**delete_item_pick_list_async**](ItemPickListsApi.md#delete_item_pick_list_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Delete an item pick list |
| [**delete_item_pick_list_entry_async**](ItemPickListsApi.md#delete_item_pick_list_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Delete a pick list entry |
| [**get_item_pick_list_by_id_async**](ItemPickListsApi.md#get_item_pick_list_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Get item pick list by ID |
| [**get_item_pick_list_entries_async**](ItemPickListsApi.md#get_item_pick_list_entries_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Get pick list entries |
| [**get_item_pick_list_entries_count_async**](ItemPickListsApi.md#get_item_pick_list_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/Count | Get pick list entries count |
| [**get_item_pick_list_entry_by_id_async**](ItemPickListsApi.md#get_item_pick_list_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Get pick list entry by ID |
| [**get_item_pick_lists_async**](ItemPickListsApi.md#get_item_pick_lists_async) | **GET** /api/v2/LogisticsService/ItemPickLists | Get all item pick lists |
| [**get_item_pick_lists_count_async**](ItemPickListsApi.md#get_item_pick_lists_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/Count | Get item pick lists count |
| [**patch_item_pick_list_async**](ItemPickListsApi.md#patch_item_pick_list_async) | **PATCH** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Patch an item pick list |
| [**patch_item_pick_list_entry_async**](ItemPickListsApi.md#patch_item_pick_list_entry_async) | **PATCH** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Patch a pick list entry |
| [**update_item_pick_list_async**](ItemPickListsApi.md#update_item_pick_list_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Update an item pick list |
| [**update_item_pick_list_entry_async**](ItemPickListsApi.md#update_item_pick_list_entry_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Update a pick list entry |


## create_item_pick_list_async

> <EmptyEnvelope> create_item_pick_list_async(tenant_id, opts)

Create an item pick list

Creates a new item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_create_dto: OpenapiClient::ItemPickListCreateDto.new({name: 'name_example'}) # ItemPickListCreateDto | 
}

begin
  # Create an item pick list
  result = api_instance.create_item_pick_list_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->create_item_pick_list_async: #{e}"
end
```

#### Using the create_item_pick_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_pick_list_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an item pick list
  data, status_code, headers = api_instance.create_item_pick_list_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->create_item_pick_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_create_dto** | [**ItemPickListCreateDto**](ItemPickListCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_item_pick_list_entry_async

> <EmptyEnvelope> create_item_pick_list_entry_async(tenant_id, pick_list_id, opts)

Create a pick list entry

Creates a new pick list entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_entry_create_dto: OpenapiClient::ItemPickListEntryCreateDto.new({item_id: 'item_id_example', warehouse_id: 'warehouse_id_example', item_pick_list_id: 'item_pick_list_id_example'}) # ItemPickListEntryCreateDto | 
}

begin
  # Create a pick list entry
  result = api_instance.create_item_pick_list_entry_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->create_item_pick_list_entry_async: #{e}"
end
```

#### Using the create_item_pick_list_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Create a pick list entry
  data, status_code, headers = api_instance.create_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->create_item_pick_list_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_entry_create_dto** | [**ItemPickListEntryCreateDto**](ItemPickListEntryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_pick_list_async

> <EmptyEnvelope> delete_item_pick_list_async(tenant_id, pick_list_id, opts)

Delete an item pick list

Deletes an item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item pick list
  result = api_instance.delete_item_pick_list_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->delete_item_pick_list_async: #{e}"
end
```

#### Using the delete_item_pick_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_pick_list_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Delete an item pick list
  data, status_code, headers = api_instance.delete_item_pick_list_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->delete_item_pick_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_item_pick_list_entry_async

> <EmptyEnvelope> delete_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, opts)

Delete a pick list entry

Deletes a pick list entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a pick list entry
  result = api_instance.delete_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->delete_item_pick_list_entry_async: #{e}"
end
```

#### Using the delete_item_pick_list_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)

```ruby
begin
  # Delete a pick list entry
  data, status_code, headers = api_instance.delete_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->delete_item_pick_list_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_pick_list_by_id_async

> <ItemPickListDtoEnvelope> get_item_pick_list_by_id_async(tenant_id, pick_list_id, opts)

Get item pick list by ID

Retrieves a specific item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item pick list by ID
  result = api_instance.get_item_pick_list_by_id_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_by_id_async: #{e}"
end
```

#### Using the get_item_pick_list_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPickListDtoEnvelope>, Integer, Hash)> get_item_pick_list_by_id_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Get item pick list by ID
  data, status_code, headers = api_instance.get_item_pick_list_by_id_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPickListDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPickListDtoEnvelope**](ItemPickListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_pick_list_entries_async

> <ItemPickListEntryDtoListEnvelope> get_item_pick_list_entries_async(tenant_id, pick_list_id, opts)

Get pick list entries

Retrieves all entries for the specified pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_entry_dto_collection_query_parameters: OpenapiClient::ItemPickListEntryDtoCollectionQueryParameters.new # ItemPickListEntryDtoCollectionQueryParameters | 
}

begin
  # Get pick list entries
  result = api_instance.get_item_pick_list_entries_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_entries_async: #{e}"
end
```

#### Using the get_item_pick_list_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPickListEntryDtoListEnvelope>, Integer, Hash)> get_item_pick_list_entries_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Get pick list entries
  data, status_code, headers = api_instance.get_item_pick_list_entries_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPickListEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_entry_dto_collection_query_parameters** | [**ItemPickListEntryDtoCollectionQueryParameters**](ItemPickListEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemPickListEntryDtoListEnvelope**](ItemPickListEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_pick_list_entries_count_async

> <Int32Envelope> get_item_pick_list_entries_count_async(tenant_id, pick_list_id, opts)

Get pick list entries count

Returns the count of pick list entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_entry_dto_collection_query_parameters: OpenapiClient::ItemPickListEntryDtoCollectionQueryParameters.new # ItemPickListEntryDtoCollectionQueryParameters | 
}

begin
  # Get pick list entries count
  result = api_instance.get_item_pick_list_entries_count_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_entries_count_async: #{e}"
end
```

#### Using the get_item_pick_list_entries_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_pick_list_entries_count_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Get pick list entries count
  data, status_code, headers = api_instance.get_item_pick_list_entries_count_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_entries_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_entry_dto_collection_query_parameters** | [**ItemPickListEntryDtoCollectionQueryParameters**](ItemPickListEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_pick_list_entry_by_id_async

> <ItemPickListEntryDtoEnvelope> get_item_pick_list_entry_by_id_async(tenant_id, pick_list_id, entry_id, opts)

Get pick list entry by ID

Retrieves a specific pick list entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get pick list entry by ID
  result = api_instance.get_item_pick_list_entry_by_id_async(tenant_id, pick_list_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_entry_by_id_async: #{e}"
end
```

#### Using the get_item_pick_list_entry_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPickListEntryDtoEnvelope>, Integer, Hash)> get_item_pick_list_entry_by_id_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)

```ruby
begin
  # Get pick list entry by ID
  data, status_code, headers = api_instance.get_item_pick_list_entry_by_id_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPickListEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_list_entry_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPickListEntryDtoEnvelope**](ItemPickListEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_pick_lists_async

> <ItemPickListDtoListEnvelope> get_item_pick_lists_async(tenant_id, opts)

Get all item pick lists

Retrieves all item pick lists for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_dto_collection_query_parameters: OpenapiClient::ItemPickListDtoCollectionQueryParameters.new # ItemPickListDtoCollectionQueryParameters | 
}

begin
  # Get all item pick lists
  result = api_instance.get_item_pick_lists_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_lists_async: #{e}"
end
```

#### Using the get_item_pick_lists_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPickListDtoListEnvelope>, Integer, Hash)> get_item_pick_lists_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item pick lists
  data, status_code, headers = api_instance.get_item_pick_lists_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPickListDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_lists_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_dto_collection_query_parameters** | [**ItemPickListDtoCollectionQueryParameters**](ItemPickListDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemPickListDtoListEnvelope**](ItemPickListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_pick_lists_count_async

> <Int32Envelope> get_item_pick_lists_count_async(tenant_id, opts)

Get item pick lists count

Returns the count of item pick lists.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_dto_collection_query_parameters: OpenapiClient::ItemPickListDtoCollectionQueryParameters.new # ItemPickListDtoCollectionQueryParameters | 
}

begin
  # Get item pick lists count
  result = api_instance.get_item_pick_lists_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_lists_count_async: #{e}"
end
```

#### Using the get_item_pick_lists_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_pick_lists_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get item pick lists count
  data, status_code, headers = api_instance.get_item_pick_lists_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->get_item_pick_lists_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_dto_collection_query_parameters** | [**ItemPickListDtoCollectionQueryParameters**](ItemPickListDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_item_pick_list_async

> <EmptyEnvelope> patch_item_pick_list_async(tenant_id, pick_list_id, opts)

Patch an item pick list

Applies a JSON Patch document to an item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an item pick list
  result = api_instance.patch_item_pick_list_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->patch_item_pick_list_async: #{e}"
end
```

#### Using the patch_item_pick_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_pick_list_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Patch an item pick list
  data, status_code, headers = api_instance.patch_item_pick_list_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->patch_item_pick_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_item_pick_list_entry_async

> <EmptyEnvelope> patch_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, opts)

Patch a pick list entry

Applies a JSON Patch document to a pick list entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a pick list entry
  result = api_instance.patch_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->patch_item_pick_list_entry_async: #{e}"
end
```

#### Using the patch_item_pick_list_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)

```ruby
begin
  # Patch a pick list entry
  data, status_code, headers = api_instance.patch_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->patch_item_pick_list_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_pick_list_async

> <EmptyEnvelope> update_item_pick_list_async(tenant_id, pick_list_id, opts)

Update an item pick list

Updates an existing item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_update_dto: OpenapiClient::ItemPickListUpdateDto.new # ItemPickListUpdateDto | 
}

begin
  # Update an item pick list
  result = api_instance.update_item_pick_list_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->update_item_pick_list_async: #{e}"
end
```

#### Using the update_item_pick_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_pick_list_async_with_http_info(tenant_id, pick_list_id, opts)

```ruby
begin
  # Update an item pick list
  data, status_code, headers = api_instance.update_item_pick_list_async_with_http_info(tenant_id, pick_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->update_item_pick_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_update_dto** | [**ItemPickListUpdateDto**](ItemPickListUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_pick_list_entry_async

> <EmptyEnvelope> update_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, opts)

Update a pick list entry

Updates an existing pick list entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPickListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_pick_list_entry_update_dto: OpenapiClient::ItemPickListEntryUpdateDto.new # ItemPickListEntryUpdateDto | 
}

begin
  # Update a pick list entry
  result = api_instance.update_item_pick_list_entry_async(tenant_id, pick_list_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->update_item_pick_list_entry_async: #{e}"
end
```

#### Using the update_item_pick_list_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)

```ruby
begin
  # Update a pick list entry
  data, status_code, headers = api_instance.update_item_pick_list_entry_async_with_http_info(tenant_id, pick_list_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPickListsApi->update_item_pick_list_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **pick_list_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_pick_list_entry_update_dto** | [**ItemPickListEntryUpdateDto**](ItemPickListEntryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

