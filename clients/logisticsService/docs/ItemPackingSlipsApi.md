# OpenapiClient::ItemPackingSlipsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_packing_slip_async**](ItemPackingSlipsApi.md#create_item_packing_slip_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips | Create an item packing slip |
| [**create_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#create_item_packing_slip_entry_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Create a packing slip entry |
| [**delete_item_packing_slip_async**](ItemPackingSlipsApi.md#delete_item_packing_slip_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Delete an item packing slip |
| [**delete_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#delete_item_packing_slip_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Delete a packing slip entry |
| [**get_item_packing_slip_by_id_async**](ItemPackingSlipsApi.md#get_item_packing_slip_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Get item packing slip by ID |
| [**get_item_packing_slip_entries_async**](ItemPackingSlipsApi.md#get_item_packing_slip_entries_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Get packing slip entries |
| [**get_item_packing_slip_entries_count_async**](ItemPackingSlipsApi.md#get_item_packing_slip_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/Count | Get packing slip entries count |
| [**get_item_packing_slip_entry_by_id_async**](ItemPackingSlipsApi.md#get_item_packing_slip_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Get packing slip entry by ID |
| [**get_item_packing_slips_async**](ItemPackingSlipsApi.md#get_item_packing_slips_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips | Get all item packing slips |
| [**get_item_packing_slips_count_async**](ItemPackingSlipsApi.md#get_item_packing_slips_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/Count | Get item packing slips count |
| [**patch_item_packing_slip_async**](ItemPackingSlipsApi.md#patch_item_packing_slip_async) | **PATCH** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Patch an item packing slip |
| [**patch_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#patch_item_packing_slip_entry_async) | **PATCH** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Patch a packing slip entry |
| [**update_item_packing_slip_async**](ItemPackingSlipsApi.md#update_item_packing_slip_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Update an item packing slip |
| [**update_item_packing_slip_entry_async**](ItemPackingSlipsApi.md#update_item_packing_slip_entry_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Update a packing slip entry |


## create_item_packing_slip_async

> <EmptyEnvelope> create_item_packing_slip_async(tenant_id, opts)

Create an item packing slip

Creates a new item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_create_dto: OpenapiClient::ItemPackingSlipCreateDto.new # ItemPackingSlipCreateDto | 
}

begin
  # Create an item packing slip
  result = api_instance.create_item_packing_slip_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->create_item_packing_slip_async: #{e}"
end
```

#### Using the create_item_packing_slip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_packing_slip_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an item packing slip
  data, status_code, headers = api_instance.create_item_packing_slip_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->create_item_packing_slip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_create_dto** | [**ItemPackingSlipCreateDto**](ItemPackingSlipCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_item_packing_slip_entry_async

> <EmptyEnvelope> create_item_packing_slip_entry_async(tenant_id, packing_slip_id, opts)

Create a packing slip entry

Creates a new packing slip entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_entry_create_dto: OpenapiClient::ItemPackingSlipEntryCreateDto.new({item_id: 'item_id_example', item_packing_slip_id: 'item_packing_slip_id_example', quantity: 'quantity_example'}) # ItemPackingSlipEntryCreateDto | 
}

begin
  # Create a packing slip entry
  result = api_instance.create_item_packing_slip_entry_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->create_item_packing_slip_entry_async: #{e}"
end
```

#### Using the create_item_packing_slip_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Create a packing slip entry
  data, status_code, headers = api_instance.create_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->create_item_packing_slip_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_entry_create_dto** | [**ItemPackingSlipEntryCreateDto**](ItemPackingSlipEntryCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_item_packing_slip_async

> <EmptyEnvelope> delete_item_packing_slip_async(tenant_id, packing_slip_id, opts)

Delete an item packing slip

Deletes an item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item packing slip
  result = api_instance.delete_item_packing_slip_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->delete_item_packing_slip_async: #{e}"
end
```

#### Using the delete_item_packing_slip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_packing_slip_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Delete an item packing slip
  data, status_code, headers = api_instance.delete_item_packing_slip_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->delete_item_packing_slip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_item_packing_slip_entry_async

> <EmptyEnvelope> delete_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, opts)

Delete a packing slip entry

Deletes a packing slip entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a packing slip entry
  result = api_instance.delete_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->delete_item_packing_slip_entry_async: #{e}"
end
```

#### Using the delete_item_packing_slip_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)

```ruby
begin
  # Delete a packing slip entry
  data, status_code, headers = api_instance.delete_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->delete_item_packing_slip_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
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


## get_item_packing_slip_by_id_async

> <ItemPackingSlipDtoEnvelope> get_item_packing_slip_by_id_async(tenant_id, packing_slip_id, opts)

Get item packing slip by ID

Retrieves a specific item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item packing slip by ID
  result = api_instance.get_item_packing_slip_by_id_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_by_id_async: #{e}"
end
```

#### Using the get_item_packing_slip_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPackingSlipDtoEnvelope>, Integer, Hash)> get_item_packing_slip_by_id_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Get item packing slip by ID
  data, status_code, headers = api_instance.get_item_packing_slip_by_id_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPackingSlipDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPackingSlipDtoEnvelope**](ItemPackingSlipDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_packing_slip_entries_async

> <ItemPackingSlipEntryDtoListEnvelope> get_item_packing_slip_entries_async(tenant_id, packing_slip_id, opts)

Get packing slip entries

Retrieves all entries for the specified packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_entry_dto_collection_query_parameters: OpenapiClient::ItemPackingSlipEntryDtoCollectionQueryParameters.new # ItemPackingSlipEntryDtoCollectionQueryParameters | 
}

begin
  # Get packing slip entries
  result = api_instance.get_item_packing_slip_entries_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_entries_async: #{e}"
end
```

#### Using the get_item_packing_slip_entries_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPackingSlipEntryDtoListEnvelope>, Integer, Hash)> get_item_packing_slip_entries_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Get packing slip entries
  data, status_code, headers = api_instance.get_item_packing_slip_entries_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPackingSlipEntryDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_entries_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_entry_dto_collection_query_parameters** | [**ItemPackingSlipEntryDtoCollectionQueryParameters**](ItemPackingSlipEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemPackingSlipEntryDtoListEnvelope**](ItemPackingSlipEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_packing_slip_entries_count_async

> <Int32Envelope> get_item_packing_slip_entries_count_async(tenant_id, packing_slip_id, opts)

Get packing slip entries count

Returns the count of packing slip entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_entry_dto_collection_query_parameters: OpenapiClient::ItemPackingSlipEntryDtoCollectionQueryParameters.new # ItemPackingSlipEntryDtoCollectionQueryParameters | 
}

begin
  # Get packing slip entries count
  result = api_instance.get_item_packing_slip_entries_count_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_entries_count_async: #{e}"
end
```

#### Using the get_item_packing_slip_entries_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_packing_slip_entries_count_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Get packing slip entries count
  data, status_code, headers = api_instance.get_item_packing_slip_entries_count_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_entries_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_entry_dto_collection_query_parameters** | [**ItemPackingSlipEntryDtoCollectionQueryParameters**](ItemPackingSlipEntryDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_packing_slip_entry_by_id_async

> <ItemPackingSlipEntryDtoEnvelope> get_item_packing_slip_entry_by_id_async(tenant_id, packing_slip_id, entry_id, opts)

Get packing slip entry by ID

Retrieves a specific packing slip entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get packing slip entry by ID
  result = api_instance.get_item_packing_slip_entry_by_id_async(tenant_id, packing_slip_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_entry_by_id_async: #{e}"
end
```

#### Using the get_item_packing_slip_entry_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPackingSlipEntryDtoEnvelope>, Integer, Hash)> get_item_packing_slip_entry_by_id_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)

```ruby
begin
  # Get packing slip entry by ID
  data, status_code, headers = api_instance.get_item_packing_slip_entry_by_id_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPackingSlipEntryDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slip_entry_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPackingSlipEntryDtoEnvelope**](ItemPackingSlipEntryDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_packing_slips_async

> <ItemPackingSlipDtoListEnvelope> get_item_packing_slips_async(tenant_id, opts)

Get all item packing slips

Retrieves all item packing slips for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_dto_collection_query_parameters: OpenapiClient::ItemPackingSlipDtoCollectionQueryParameters.new # ItemPackingSlipDtoCollectionQueryParameters | 
}

begin
  # Get all item packing slips
  result = api_instance.get_item_packing_slips_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slips_async: #{e}"
end
```

#### Using the get_item_packing_slips_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPackingSlipDtoListEnvelope>, Integer, Hash)> get_item_packing_slips_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item packing slips
  data, status_code, headers = api_instance.get_item_packing_slips_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPackingSlipDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slips_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_dto_collection_query_parameters** | [**ItemPackingSlipDtoCollectionQueryParameters**](ItemPackingSlipDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**ItemPackingSlipDtoListEnvelope**](ItemPackingSlipDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_packing_slips_count_async

> <Int32Envelope> get_item_packing_slips_count_async(tenant_id, opts)

Get item packing slips count

Returns the count of item packing slips.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_dto_collection_query_parameters: OpenapiClient::ItemPackingSlipDtoCollectionQueryParameters.new # ItemPackingSlipDtoCollectionQueryParameters | 
}

begin
  # Get item packing slips count
  result = api_instance.get_item_packing_slips_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slips_count_async: #{e}"
end
```

#### Using the get_item_packing_slips_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_packing_slips_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get item packing slips count
  data, status_code, headers = api_instance.get_item_packing_slips_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->get_item_packing_slips_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_dto_collection_query_parameters** | [**ItemPackingSlipDtoCollectionQueryParameters**](ItemPackingSlipDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_item_packing_slip_async

> <EmptyEnvelope> patch_item_packing_slip_async(tenant_id, packing_slip_id, opts)

Patch an item packing slip

Applies a JSON Patch document to an item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch an item packing slip
  result = api_instance.patch_item_packing_slip_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->patch_item_packing_slip_async: #{e}"
end
```

#### Using the patch_item_packing_slip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_packing_slip_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Patch an item packing slip
  data, status_code, headers = api_instance.patch_item_packing_slip_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->patch_item_packing_slip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
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


## patch_item_packing_slip_entry_async

> <EmptyEnvelope> patch_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, opts)

Patch a packing slip entry

Applies a JSON Patch document to a packing slip entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a packing slip entry
  result = api_instance.patch_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->patch_item_packing_slip_entry_async: #{e}"
end
```

#### Using the patch_item_packing_slip_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)

```ruby
begin
  # Patch a packing slip entry
  data, status_code, headers = api_instance.patch_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->patch_item_packing_slip_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
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


## update_item_packing_slip_async

> <EmptyEnvelope> update_item_packing_slip_async(tenant_id, packing_slip_id, opts)

Update an item packing slip

Updates an existing item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_update_dto: OpenapiClient::ItemPackingSlipUpdateDto.new # ItemPackingSlipUpdateDto | 
}

begin
  # Update an item packing slip
  result = api_instance.update_item_packing_slip_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->update_item_packing_slip_async: #{e}"
end
```

#### Using the update_item_packing_slip_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_packing_slip_async_with_http_info(tenant_id, packing_slip_id, opts)

```ruby
begin
  # Update an item packing slip
  data, status_code, headers = api_instance.update_item_packing_slip_async_with_http_info(tenant_id, packing_slip_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->update_item_packing_slip_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_update_dto** | [**ItemPackingSlipUpdateDto**](ItemPackingSlipUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_item_packing_slip_entry_async

> <EmptyEnvelope> update_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, opts)

Update a packing slip entry

Updates an existing packing slip entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ItemPackingSlipsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
entry_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_packing_slip_entry_update_dto: OpenapiClient::ItemPackingSlipEntryUpdateDto.new # ItemPackingSlipEntryUpdateDto | 
}

begin
  # Update a packing slip entry
  result = api_instance.update_item_packing_slip_entry_async(tenant_id, packing_slip_id, entry_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->update_item_packing_slip_entry_async: #{e}"
end
```

#### Using the update_item_packing_slip_entry_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)

```ruby
begin
  # Update a packing slip entry
  data, status_code, headers = api_instance.update_item_packing_slip_entry_async_with_http_info(tenant_id, packing_slip_id, entry_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ItemPackingSlipsApi->update_item_packing_slip_entry_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **packing_slip_id** | **String** |  |  |
| **entry_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_packing_slip_entry_update_dto** | [**ItemPackingSlipEntryUpdateDto**](ItemPackingSlipEntryUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

