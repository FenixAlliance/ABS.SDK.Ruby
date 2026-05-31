# OpenapiClient::ItemRestocksApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_restock_async**](ItemRestocksApi.md#create_item_restock_async) | **POST** /api/v2/LogisticsService/ItemRestocks | Create an item restock |
| [**create_item_restock_entry_async**](ItemRestocksApi.md#create_item_restock_entry_async) | **POST** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Create a restock entry |
| [**delete_item_restock_async**](ItemRestocksApi.md#delete_item_restock_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId} | Delete an item restock |
| [**delete_item_restock_entry_async**](ItemRestocksApi.md#delete_item_restock_entry_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Delete a restock entry |
| [**get_item_restock_by_id_async**](ItemRestocksApi.md#get_item_restock_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId} | Get item restock by ID |
| [**get_item_restock_entries_async**](ItemRestocksApi.md#get_item_restock_entries_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Get restock entries |
| [**get_item_restock_entries_count_async**](ItemRestocksApi.md#get_item_restock_entries_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/Count | Get restock entries count |
| [**get_item_restock_entry_by_id_async**](ItemRestocksApi.md#get_item_restock_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Get restock entry by ID |
| [**get_item_restocks_async**](ItemRestocksApi.md#get_item_restocks_async) | **GET** /api/v2/LogisticsService/ItemRestocks | Get all item restocks |
| [**get_item_restocks_count_async**](ItemRestocksApi.md#get_item_restocks_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/Count | Get item restocks count |
| [**update_item_restock_async**](ItemRestocksApi.md#update_item_restock_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId} | Update an item restock |
| [**update_item_restock_entry_async**](ItemRestocksApi.md#update_item_restock_entry_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Update a restock entry |


## create_item_restock_async

> <EmptyEnvelope> create_item_restock_async(tenant_id, opts)

Create an item restock

Creates a new item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_restock_create_dto: OpenapiClient::ItemRestockCreateDto.new # ItemRestockCreateDto | 
}

begin
  # Create an item restock
  result = api_instance.create_item_restock_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->create_item_restock_async: #{e}"
end
```

#### Using the create_item_restock_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_restock_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an item restock
  data, status_code, headers = api_instance.create_item_restock_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->create_item_restock_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_restock_create_dto** | [**ItemRestockCreateDto**](ItemRestockCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_item_restock_entry_async

> <EmptyEnvelope> create_item_restock_entry_async(tenant_id, restock_id, opts)

Create a restock entry

Creates a new restock entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_restock_entry_create_dto: OpenapiClient::ItemRestockEntryCreateDto.new({item_id: 'item_id_example', warehouse_id: 'warehouse_id_example', item_restock_id: 'item_restock_id_example'}) # ItemRestockEntryCreateDto | 
}

begin
  # Create a restock entry
  result = api_instance.create_item_restock_entry_async(tenant_id, restock_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->create_item_restock_entry_async: #{e}"
end
```

#### Using the create_item_restock_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_restock_entry_async_with_http_info(tenant_id, restock_id, opts)

```ruby
begin
  # Create a restock entry
  data, status_code, headers = api_instance.create_item_restock_entry_async_with_http_info(tenant_id, restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->create_item_restock_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_restock_entry_create_dto** | [**ItemRestockEntryCreateDto**](ItemRestockEntryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_restock_async

> <EmptyEnvelope> delete_item_restock_async(tenant_id, restock_id, opts)

Delete an item restock

Deletes an item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item restock
  result = api_instance.delete_item_restock_async(tenant_id, restock_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->delete_item_restock_async: #{e}"
end
```

#### Using the delete_item_restock_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_restock_async_with_http_info(tenant_id, restock_id, opts)

```ruby
begin
  # Delete an item restock
  data, status_code, headers = api_instance.delete_item_restock_async_with_http_info(tenant_id, restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->delete_item_restock_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_item_restock_entry_async

> <EmptyEnvelope> delete_item_restock_entry_async(tenant_id, restock_id, entry_id, opts)

Delete a restock entry

Deletes a restock entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a restock entry
  result = api_instance.delete_item_restock_entry_async(tenant_id, restock_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->delete_item_restock_entry_async: #{e}"
end
```

#### Using the delete_item_restock_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_restock_entry_async_with_http_info(tenant_id, restock_id, entry_id, opts)

```ruby
begin
  # Delete a restock entry
  data, status_code, headers = api_instance.delete_item_restock_entry_async_with_http_info(tenant_id, restock_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->delete_item_restock_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
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


## get_item_restock_by_id_async

> <ItemRestockDtoEnvelope> get_item_restock_by_id_async(tenant_id, restock_id, opts)

Get item restock by ID

Retrieves a specific item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item restock by ID
  result = api_instance.get_item_restock_by_id_async(tenant_id, restock_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_by_id_async: #{e}"
end
```

#### Using the get_item_restock_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRestockDtoEnvelope>, Integer, Hash)> get_item_restock_by_id_async_with_http_info(tenant_id, restock_id, opts)

```ruby
begin
  # Get item restock by ID
  data, status_code, headers = api_instance.get_item_restock_by_id_async_with_http_info(tenant_id, restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRestockDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRestockDtoEnvelope**](ItemRestockDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_restock_entries_async

> <ItemRestockEntryDtoListEnvelope> get_item_restock_entries_async(tenant_id, restock_id, opts)

Get restock entries

Retrieves all entries for the specified restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get restock entries
  result = api_instance.get_item_restock_entries_async(tenant_id, restock_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_entries_async: #{e}"
end
```

#### Using the get_item_restock_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRestockEntryDtoListEnvelope>, Integer, Hash)> get_item_restock_entries_async_with_http_info(tenant_id, restock_id, opts)

```ruby
begin
  # Get restock entries
  data, status_code, headers = api_instance.get_item_restock_entries_async_with_http_info(tenant_id, restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRestockEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRestockEntryDtoListEnvelope**](ItemRestockEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_restock_entries_count_async

> <Int32Envelope> get_item_restock_entries_count_async(tenant_id, restock_id, opts)

Get restock entries count

Returns the count of restock entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get restock entries count
  result = api_instance.get_item_restock_entries_count_async(tenant_id, restock_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_entries_count_async: #{e}"
end
```

#### Using the get_item_restock_entries_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_restock_entries_count_async_with_http_info(tenant_id, restock_id, opts)

```ruby
begin
  # Get restock entries count
  data, status_code, headers = api_instance.get_item_restock_entries_count_async_with_http_info(tenant_id, restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_entries_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_restock_entry_by_id_async

> <ItemRestockEntryDtoEnvelope> get_item_restock_entry_by_id_async(tenant_id, restock_id, entry_id, opts)

Get restock entry by ID

Retrieves a specific restock entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get restock entry by ID
  result = api_instance.get_item_restock_entry_by_id_async(tenant_id, restock_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_entry_by_id_async: #{e}"
end
```

#### Using the get_item_restock_entry_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRestockEntryDtoEnvelope>, Integer, Hash)> get_item_restock_entry_by_id_async_with_http_info(tenant_id, restock_id, entry_id, opts)

```ruby
begin
  # Get restock entry by ID
  data, status_code, headers = api_instance.get_item_restock_entry_by_id_async_with_http_info(tenant_id, restock_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRestockEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restock_entry_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRestockEntryDtoEnvelope**](ItemRestockEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_restocks_async

> <ItemRestockDtoListEnvelope> get_item_restocks_async(tenant_id, opts)

Get all item restocks

Retrieves all item restocks for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item restocks
  result = api_instance.get_item_restocks_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restocks_async: #{e}"
end
```

#### Using the get_item_restocks_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRestockDtoListEnvelope>, Integer, Hash)> get_item_restocks_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item restocks
  data, status_code, headers = api_instance.get_item_restocks_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRestockDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restocks_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRestockDtoListEnvelope**](ItemRestockDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_restocks_count_async

> <Int32Envelope> get_item_restocks_count_async(tenant_id, opts)

Get item restocks count

Returns the count of item restocks.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item restocks count
  result = api_instance.get_item_restocks_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restocks_count_async: #{e}"
end
```

#### Using the get_item_restocks_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_restocks_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get item restocks count
  data, status_code, headers = api_instance.get_item_restocks_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->get_item_restocks_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## update_item_restock_async

> <EmptyEnvelope> update_item_restock_async(tenant_id, restock_id, opts)

Update an item restock

Updates an existing item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_restock_update_dto: OpenapiClient::ItemRestockUpdateDto.new # ItemRestockUpdateDto | 
}

begin
  # Update an item restock
  result = api_instance.update_item_restock_async(tenant_id, restock_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->update_item_restock_async: #{e}"
end
```

#### Using the update_item_restock_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_restock_async_with_http_info(tenant_id, restock_id, opts)

```ruby
begin
  # Update an item restock
  data, status_code, headers = api_instance.update_item_restock_async_with_http_info(tenant_id, restock_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->update_item_restock_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_restock_update_dto** | [**ItemRestockUpdateDto**](ItemRestockUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_restock_entry_async

> <EmptyEnvelope> update_item_restock_entry_async(tenant_id, restock_id, entry_id, opts)

Update a restock entry

Updates an existing restock entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemRestocksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
restock_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_restock_entry_update_dto: OpenapiClient::ItemRestockEntryUpdateDto.new # ItemRestockEntryUpdateDto | 
}

begin
  # Update a restock entry
  result = api_instance.update_item_restock_entry_async(tenant_id, restock_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->update_item_restock_entry_async: #{e}"
end
```

#### Using the update_item_restock_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_restock_entry_async_with_http_info(tenant_id, restock_id, entry_id, opts)

```ruby
begin
  # Update a restock entry
  data, status_code, headers = api_instance.update_item_restock_entry_async_with_http_info(tenant_id, restock_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemRestocksApi->update_item_restock_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **restock_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_restock_entry_update_dto** | [**ItemRestockEntryUpdateDto**](ItemRestockEntryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

