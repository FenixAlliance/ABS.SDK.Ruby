# OpenapiClient::WarehousingApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_item_packing_slip_async**](WarehousingApi.md#create_item_packing_slip_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips | Create an item packing slip |
| [**create_item_packing_slip_entry_async**](WarehousingApi.md#create_item_packing_slip_entry_async) | **POST** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Create a packing slip entry |
| [**create_item_pick_list_async**](WarehousingApi.md#create_item_pick_list_async) | **POST** /api/v2/LogisticsService/ItemPickLists | Create an item pick list |
| [**create_item_pick_list_entry_async**](WarehousingApi.md#create_item_pick_list_entry_async) | **POST** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Create a pick list entry |
| [**create_item_restock_async**](WarehousingApi.md#create_item_restock_async) | **POST** /api/v2/LogisticsService/ItemRestocks | Create an item restock |
| [**create_item_restock_entry_async**](WarehousingApi.md#create_item_restock_entry_async) | **POST** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Create a restock entry |
| [**create_item_retain_sample_async**](WarehousingApi.md#create_item_retain_sample_async) | **POST** /api/v2/LogisticsService/ItemRetainSamples | Create an item retain sample |
| [**create_warehouse_async**](WarehousingApi.md#create_warehouse_async) | **POST** /api/v2/LogisticsService/Warehouses | Create a warehouse |
| [**delete_item_packing_slip_async**](WarehousingApi.md#delete_item_packing_slip_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Delete an item packing slip |
| [**delete_item_packing_slip_entry_async**](WarehousingApi.md#delete_item_packing_slip_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Delete a packing slip entry |
| [**delete_item_pick_list_async**](WarehousingApi.md#delete_item_pick_list_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Delete an item pick list |
| [**delete_item_pick_list_entry_async**](WarehousingApi.md#delete_item_pick_list_entry_async) | **DELETE** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Delete a pick list entry |
| [**delete_item_restock_async**](WarehousingApi.md#delete_item_restock_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId} | Delete an item restock |
| [**delete_item_restock_entry_async**](WarehousingApi.md#delete_item_restock_entry_async) | **DELETE** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Delete a restock entry |
| [**delete_item_retain_sample_async**](WarehousingApi.md#delete_item_retain_sample_async) | **DELETE** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Delete an item retain sample |
| [**delete_warehouse_async**](WarehousingApi.md#delete_warehouse_async) | **DELETE** /api/v2/LogisticsService/Warehouses/{warehouseId} | Delete a warehouse |
| [**get_item_packing_slip_by_id_async**](WarehousingApi.md#get_item_packing_slip_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Get item packing slip by ID |
| [**get_item_packing_slip_entries_async**](WarehousingApi.md#get_item_packing_slip_entries_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries | Get packing slip entries |
| [**get_item_packing_slip_entries_count_async**](WarehousingApi.md#get_item_packing_slip_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/Count | Get packing slip entries count |
| [**get_item_packing_slip_entry_by_id_async**](WarehousingApi.md#get_item_packing_slip_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Get packing slip entry by ID |
| [**get_item_packing_slips_async**](WarehousingApi.md#get_item_packing_slips_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips | Get all item packing slips |
| [**get_item_packing_slips_count_async**](WarehousingApi.md#get_item_packing_slips_count_async) | **GET** /api/v2/LogisticsService/ItemPackingSlips/Count | Get item packing slips count |
| [**get_item_pick_list_by_id_async**](WarehousingApi.md#get_item_pick_list_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Get item pick list by ID |
| [**get_item_pick_list_entries_async**](WarehousingApi.md#get_item_pick_list_entries_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries | Get pick list entries |
| [**get_item_pick_list_entries_count_async**](WarehousingApi.md#get_item_pick_list_entries_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/Count | Get pick list entries count |
| [**get_item_pick_list_entry_by_id_async**](WarehousingApi.md#get_item_pick_list_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Get pick list entry by ID |
| [**get_item_pick_lists_async**](WarehousingApi.md#get_item_pick_lists_async) | **GET** /api/v2/LogisticsService/ItemPickLists | Get all item pick lists |
| [**get_item_pick_lists_count_async**](WarehousingApi.md#get_item_pick_lists_count_async) | **GET** /api/v2/LogisticsService/ItemPickLists/Count | Get item pick lists count |
| [**get_item_restock_by_id_async**](WarehousingApi.md#get_item_restock_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId} | Get item restock by ID |
| [**get_item_restock_entries_async**](WarehousingApi.md#get_item_restock_entries_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries | Get restock entries |
| [**get_item_restock_entries_count_async**](WarehousingApi.md#get_item_restock_entries_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/Count | Get restock entries count |
| [**get_item_restock_entry_by_id_async**](WarehousingApi.md#get_item_restock_entry_by_id_async) | **GET** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Get restock entry by ID |
| [**get_item_restocks_async**](WarehousingApi.md#get_item_restocks_async) | **GET** /api/v2/LogisticsService/ItemRestocks | Get all item restocks |
| [**get_item_restocks_count_async**](WarehousingApi.md#get_item_restocks_count_async) | **GET** /api/v2/LogisticsService/ItemRestocks/Count | Get item restocks count |
| [**get_item_retain_sample_by_id_async**](WarehousingApi.md#get_item_retain_sample_by_id_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Get item retain sample by ID |
| [**get_item_retain_samples_async**](WarehousingApi.md#get_item_retain_samples_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples | Get all item retain samples |
| [**get_item_retain_samples_count_async**](WarehousingApi.md#get_item_retain_samples_count_async) | **GET** /api/v2/LogisticsService/ItemRetainSamples/Count | Get item retain samples count |
| [**get_warehouse_by_id_async**](WarehousingApi.md#get_warehouse_by_id_async) | **GET** /api/v2/LogisticsService/Warehouses/{warehouseId} | Get warehouse by ID |
| [**get_warehouses_async**](WarehousingApi.md#get_warehouses_async) | **GET** /api/v2/LogisticsService/Warehouses | Get all warehouses |
| [**get_warehouses_count_async**](WarehousingApi.md#get_warehouses_count_async) | **GET** /api/v2/LogisticsService/Warehouses/Count | Get warehouses count |
| [**update_item_packing_slip_async**](WarehousingApi.md#update_item_packing_slip_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId} | Update an item packing slip |
| [**update_item_packing_slip_entry_async**](WarehousingApi.md#update_item_packing_slip_entry_async) | **PUT** /api/v2/LogisticsService/ItemPackingSlips/{packingSlipId}/Entries/{entryId} | Update a packing slip entry |
| [**update_item_pick_list_async**](WarehousingApi.md#update_item_pick_list_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId} | Update an item pick list |
| [**update_item_pick_list_entry_async**](WarehousingApi.md#update_item_pick_list_entry_async) | **PUT** /api/v2/LogisticsService/ItemPickLists/{pickListId}/Entries/{entryId} | Update a pick list entry |
| [**update_item_restock_async**](WarehousingApi.md#update_item_restock_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId} | Update an item restock |
| [**update_item_restock_entry_async**](WarehousingApi.md#update_item_restock_entry_async) | **PUT** /api/v2/LogisticsService/ItemRestocks/{restockId}/Entries/{entryId} | Update a restock entry |
| [**update_item_retain_sample_async**](WarehousingApi.md#update_item_retain_sample_async) | **PUT** /api/v2/LogisticsService/ItemRetainSamples/{retainSampleId} | Update an item retain sample |
| [**update_warehouse_async**](WarehousingApi.md#update_warehouse_async) | **PUT** /api/v2/LogisticsService/Warehouses/{warehouseId} | Update a warehouse |


## create_item_packing_slip_async

> <EmptyEnvelope> create_item_packing_slip_async(tenant_id, opts)

Create an item packing slip

Creates a new item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->create_item_packing_slip_async: #{e}"
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
  puts "Error when calling WarehousingApi->create_item_packing_slip_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->create_item_packing_slip_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->create_item_packing_slip_entry_async_with_http_info: #{e}"
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


## create_item_pick_list_async

> <EmptyEnvelope> create_item_pick_list_async(tenant_id, opts)

Create an item pick list

Creates a new item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->create_item_pick_list_async: #{e}"
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
  puts "Error when calling WarehousingApi->create_item_pick_list_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->create_item_pick_list_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->create_item_pick_list_entry_async_with_http_info: #{e}"
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


## create_item_restock_async

> <EmptyEnvelope> create_item_restock_async(tenant_id, opts)

Create an item restock

Creates a new item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->create_item_restock_async: #{e}"
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
  puts "Error when calling WarehousingApi->create_item_restock_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->create_item_restock_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->create_item_restock_entry_async_with_http_info: #{e}"
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


## create_item_retain_sample_async

> <EmptyEnvelope> create_item_retain_sample_async(tenant_id, opts)

Create an item retain sample

Creates a new item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_retain_sample_create_dto: OpenapiClient::ItemRetainSampleCreateDto.new({warehouse_id: 'warehouse_id_example', item_id: 'item_id_example'}) # ItemRetainSampleCreateDto | 
}

begin
  # Create an item retain sample
  result = api_instance.create_item_retain_sample_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->create_item_retain_sample_async: #{e}"
end
```

#### Using the create_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_item_retain_sample_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create an item retain sample
  data, status_code, headers = api_instance.create_item_retain_sample_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->create_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_retain_sample_create_dto** | [**ItemRetainSampleCreateDto**](ItemRetainSampleCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_warehouse_async

> <EmptyEnvelope> create_warehouse_async(tenant_id, opts)

Create a warehouse

Creates a new warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warehouse_create_dto: OpenapiClient::WarehouseCreateDto.new({title: 'title_example', address1: 'address1_example'}) # WarehouseCreateDto | 
}

begin
  # Create a warehouse
  result = api_instance.create_warehouse_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->create_warehouse_async: #{e}"
end
```

#### Using the create_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_warehouse_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a warehouse
  data, status_code, headers = api_instance.create_warehouse_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->create_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warehouse_create_dto** | [**WarehouseCreateDto**](WarehouseCreateDto.md) |  | [optional] |

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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->delete_item_packing_slip_async: #{e}"
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
  puts "Error when calling WarehousingApi->delete_item_packing_slip_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->delete_item_packing_slip_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->delete_item_packing_slip_entry_async_with_http_info: #{e}"
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


## delete_item_pick_list_async

> <EmptyEnvelope> delete_item_pick_list_async(tenant_id, pick_list_id, opts)

Delete an item pick list

Deletes an item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->delete_item_pick_list_async: #{e}"
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
  puts "Error when calling WarehousingApi->delete_item_pick_list_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->delete_item_pick_list_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->delete_item_pick_list_entry_async_with_http_info: #{e}"
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


## delete_item_restock_async

> <EmptyEnvelope> delete_item_restock_async(tenant_id, restock_id, opts)

Delete an item restock

Deletes an item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->delete_item_restock_async: #{e}"
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
  puts "Error when calling WarehousingApi->delete_item_restock_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->delete_item_restock_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->delete_item_restock_entry_async_with_http_info: #{e}"
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


## delete_item_retain_sample_async

> <EmptyEnvelope> delete_item_retain_sample_async(tenant_id, retain_sample_id, opts)

Delete an item retain sample

Deletes an item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an item retain sample
  result = api_instance.delete_item_retain_sample_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->delete_item_retain_sample_async: #{e}"
end
```

#### Using the delete_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Delete an item retain sample
  data, status_code, headers = api_instance.delete_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->delete_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_warehouse_async

> <EmptyEnvelope> delete_warehouse_async(tenant_id, warehouse_id, opts)

Delete a warehouse

Deletes a warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a warehouse
  result = api_instance.delete_warehouse_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->delete_warehouse_async: #{e}"
end
```

#### Using the delete_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Delete a warehouse
  data, status_code, headers = api_instance.delete_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->delete_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_packing_slip_by_id_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_packing_slip_by_id_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get packing slip entries
  result = api_instance.get_item_packing_slip_entries_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_packing_slip_entries_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_packing_slip_entries_async_with_http_info: #{e}"
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

[**ItemPackingSlipEntryDtoListEnvelope**](ItemPackingSlipEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_packing_slip_entries_count_async

> <Int32Envelope> get_item_packing_slip_entries_count_async(tenant_id, packing_slip_id, opts)

Get packing slip entries count

Returns the count of packing slip entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
packing_slip_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get packing slip entries count
  result = api_instance.get_item_packing_slip_entries_count_async(tenant_id, packing_slip_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_packing_slip_entries_count_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_packing_slip_entries_count_async_with_http_info: #{e}"
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

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_packing_slip_entry_by_id_async

> <ItemPackingSlipEntryDtoEnvelope> get_item_packing_slip_entry_by_id_async(tenant_id, packing_slip_id, entry_id, opts)

Get packing slip entry by ID

Retrieves a specific packing slip entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_packing_slip_entry_by_id_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_packing_slip_entry_by_id_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item packing slips
  result = api_instance.get_item_packing_slips_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_packing_slips_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_packing_slips_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPackingSlipDtoListEnvelope**](ItemPackingSlipDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_packing_slips_count_async

> <Int32Envelope> get_item_packing_slips_count_async(tenant_id, opts)

Get item packing slips count

Returns the count of item packing slips.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item packing slips count
  result = api_instance.get_item_packing_slips_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_packing_slips_count_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_packing_slips_count_async_with_http_info: #{e}"
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


## get_item_pick_list_by_id_async

> <ItemPickListDtoEnvelope> get_item_pick_list_by_id_async(tenant_id, pick_list_id, opts)

Get item pick list by ID

Retrieves a specific item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_pick_list_by_id_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_pick_list_by_id_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get pick list entries
  result = api_instance.get_item_pick_list_entries_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_pick_list_entries_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_pick_list_entries_async_with_http_info: #{e}"
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

[**ItemPickListEntryDtoListEnvelope**](ItemPickListEntryDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_pick_list_entries_count_async

> <Int32Envelope> get_item_pick_list_entries_count_async(tenant_id, pick_list_id, opts)

Get pick list entries count

Returns the count of pick list entries.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
pick_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get pick list entries count
  result = api_instance.get_item_pick_list_entries_count_async(tenant_id, pick_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_pick_list_entries_count_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_pick_list_entries_count_async_with_http_info: #{e}"
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

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_pick_list_entry_by_id_async

> <ItemPickListEntryDtoEnvelope> get_item_pick_list_entry_by_id_async(tenant_id, pick_list_id, entry_id, opts)

Get pick list entry by ID

Retrieves a specific pick list entry.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_pick_list_entry_by_id_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_pick_list_entry_by_id_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item pick lists
  result = api_instance.get_item_pick_lists_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_pick_lists_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_pick_lists_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemPickListDtoListEnvelope**](ItemPickListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_pick_lists_count_async

> <Int32Envelope> get_item_pick_lists_count_async(tenant_id, opts)

Get item pick lists count

Returns the count of item pick lists.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item pick lists count
  result = api_instance.get_item_pick_lists_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_pick_lists_count_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_pick_lists_count_async_with_http_info: #{e}"
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


## get_item_restock_by_id_async

> <ItemRestockDtoEnvelope> get_item_restock_by_id_async(tenant_id, restock_id, opts)

Get item restock by ID

Retrieves a specific item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_restock_by_id_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_restock_by_id_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_restock_entries_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_restock_entries_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_restock_entries_count_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_restock_entries_count_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_restock_entry_by_id_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_restock_entry_by_id_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_restocks_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_restocks_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->get_item_restocks_count_async: #{e}"
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
  puts "Error when calling WarehousingApi->get_item_restocks_count_async_with_http_info: #{e}"
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


## get_item_retain_sample_by_id_async

> <ItemRetainSampleDtoEnvelope> get_item_retain_sample_by_id_async(tenant_id, retain_sample_id, opts)

Get item retain sample by ID

Retrieves a specific item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item retain sample by ID
  result = api_instance.get_item_retain_sample_by_id_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_retain_sample_by_id_async: #{e}"
end
```

#### Using the get_item_retain_sample_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRetainSampleDtoEnvelope>, Integer, Hash)> get_item_retain_sample_by_id_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Get item retain sample by ID
  data, status_code, headers = api_instance.get_item_retain_sample_by_id_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRetainSampleDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_retain_sample_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRetainSampleDtoEnvelope**](ItemRetainSampleDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_retain_samples_async

> <ItemRetainSampleDtoListEnvelope> get_item_retain_samples_async(tenant_id, opts)

Get all item retain samples

Retrieves all item retain samples for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all item retain samples
  result = api_instance.get_item_retain_samples_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_retain_samples_async: #{e}"
end
```

#### Using the get_item_retain_samples_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemRetainSampleDtoListEnvelope>, Integer, Hash)> get_item_retain_samples_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all item retain samples
  data, status_code, headers = api_instance.get_item_retain_samples_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemRetainSampleDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_retain_samples_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemRetainSampleDtoListEnvelope**](ItemRetainSampleDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_retain_samples_count_async

> <Int32Envelope> get_item_retain_samples_count_async(tenant_id, opts)

Get item retain samples count

Returns the count of item retain samples.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get item retain samples count
  result = api_instance.get_item_retain_samples_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_retain_samples_count_async: #{e}"
end
```

#### Using the get_item_retain_samples_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_item_retain_samples_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get item retain samples count
  data, status_code, headers = api_instance.get_item_retain_samples_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_item_retain_samples_count_async_with_http_info: #{e}"
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


## get_warehouse_by_id_async

> <WarehouseDtoEnvelope> get_warehouse_by_id_async(tenant_id, warehouse_id, opts)

Get warehouse by ID

Retrieves a specific warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warehouse by ID
  result = api_instance.get_warehouse_by_id_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_warehouse_by_id_async: #{e}"
end
```

#### Using the get_warehouse_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarehouseDtoEnvelope>, Integer, Hash)> get_warehouse_by_id_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Get warehouse by ID
  data, status_code, headers = api_instance.get_warehouse_by_id_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarehouseDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_warehouse_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarehouseDtoEnvelope**](WarehouseDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warehouses_async

> <WarehouseDtoListEnvelope> get_warehouses_async(tenant_id, opts)

Get all warehouses

Retrieves all warehouses for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all warehouses
  result = api_instance.get_warehouses_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_warehouses_async: #{e}"
end
```

#### Using the get_warehouses_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WarehouseDtoListEnvelope>, Integer, Hash)> get_warehouses_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all warehouses
  data, status_code, headers = api_instance.get_warehouses_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WarehouseDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_warehouses_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WarehouseDtoListEnvelope**](WarehouseDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_warehouses_count_async

> <Int32Envelope> get_warehouses_count_async(tenant_id, opts)

Get warehouses count

Returns the count of warehouses.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get warehouses count
  result = api_instance.get_warehouses_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_warehouses_count_async: #{e}"
end
```

#### Using the get_warehouses_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_warehouses_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get warehouses count
  data, status_code, headers = api_instance.get_warehouses_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->get_warehouses_count_async_with_http_info: #{e}"
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


## update_item_packing_slip_async

> <EmptyEnvelope> update_item_packing_slip_async(tenant_id, packing_slip_id, opts)

Update an item packing slip

Updates an existing item packing slip.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->update_item_packing_slip_async: #{e}"
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
  puts "Error when calling WarehousingApi->update_item_packing_slip_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->update_item_packing_slip_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->update_item_packing_slip_entry_async_with_http_info: #{e}"
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


## update_item_pick_list_async

> <EmptyEnvelope> update_item_pick_list_async(tenant_id, pick_list_id, opts)

Update an item pick list

Updates an existing item pick list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->update_item_pick_list_async: #{e}"
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
  puts "Error when calling WarehousingApi->update_item_pick_list_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->update_item_pick_list_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->update_item_pick_list_entry_async_with_http_info: #{e}"
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


## update_item_restock_async

> <EmptyEnvelope> update_item_restock_async(tenant_id, restock_id, opts)

Update an item restock

Updates an existing item restock.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->update_item_restock_async: #{e}"
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
  puts "Error when calling WarehousingApi->update_item_restock_async_with_http_info: #{e}"
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

api_instance = OpenapiClient::WarehousingApi.new
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
  puts "Error when calling WarehousingApi->update_item_restock_entry_async: #{e}"
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
  puts "Error when calling WarehousingApi->update_item_restock_entry_async_with_http_info: #{e}"
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


## update_item_retain_sample_async

> <EmptyEnvelope> update_item_retain_sample_async(tenant_id, retain_sample_id, opts)

Update an item retain sample

Updates an existing item retain sample.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
retain_sample_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  item_retain_sample_update_dto: OpenapiClient::ItemRetainSampleUpdateDto.new # ItemRetainSampleUpdateDto | 
}

begin
  # Update an item retain sample
  result = api_instance.update_item_retain_sample_async(tenant_id, retain_sample_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->update_item_retain_sample_async: #{e}"
end
```

#### Using the update_item_retain_sample_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)

```ruby
begin
  # Update an item retain sample
  data, status_code, headers = api_instance.update_item_retain_sample_async_with_http_info(tenant_id, retain_sample_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->update_item_retain_sample_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **retain_sample_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **item_retain_sample_update_dto** | [**ItemRetainSampleUpdateDto**](ItemRetainSampleUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_warehouse_async

> <EmptyEnvelope> update_warehouse_async(tenant_id, warehouse_id, opts)

Update a warehouse

Updates an existing warehouse.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WarehousingApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
warehouse_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  warehouse_update_dto: OpenapiClient::WarehouseUpdateDto.new # WarehouseUpdateDto | 
}

begin
  # Update a warehouse
  result = api_instance.update_warehouse_async(tenant_id, warehouse_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->update_warehouse_async: #{e}"
end
```

#### Using the update_warehouse_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)

```ruby
begin
  # Update a warehouse
  data, status_code, headers = api_instance.update_warehouse_async_with_http_info(tenant_id, warehouse_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WarehousingApi->update_warehouse_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **warehouse_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **warehouse_update_dto** | [**WarehouseUpdateDto**](WarehouseUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

