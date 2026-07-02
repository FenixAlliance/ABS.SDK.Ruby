# OpenapiClient::AssetTransfersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_asset_transfer_async**](AssetTransfersApi.md#create_asset_transfer_async) | **POST** /api/v2/AssetsService/AssetTransfers | Creates a new asset transfer |
| [**delete_asset_transfer_async**](AssetTransfersApi.md#delete_asset_transfer_async) | **DELETE** /api/v2/AssetsService/AssetTransfers/{transferId} | Deletes an asset transfer |
| [**get_asset_transfer_async**](AssetTransfersApi.md#get_asset_transfer_async) | **GET** /api/v2/AssetsService/AssetTransfers/{transferId} | Gets a single asset transfer by ID |
| [**get_asset_transfers_async**](AssetTransfersApi.md#get_asset_transfers_async) | **GET** /api/v2/AssetsService/AssetTransfers | Gets a list of asset transfers |
| [**get_asset_transfers_count_async**](AssetTransfersApi.md#get_asset_transfers_count_async) | **GET** /api/v2/AssetsService/AssetTransfers/Count | Gets the count of asset transfers |
| [**patch_asset_transfer_async**](AssetTransfersApi.md#patch_asset_transfer_async) | **PATCH** /api/v2/AssetsService/AssetTransfers/{transferId} | Partially updates an existing asset transfer |
| [**update_asset_transfer_async**](AssetTransfersApi.md#update_asset_transfer_async) | **PUT** /api/v2/AssetsService/AssetTransfers/{transferId} | Updates an existing asset transfer |


## create_asset_transfer_async

> <EmptyEnvelope> create_asset_transfer_async(tenant_id, opts)

Creates a new asset transfer

Creates a new asset transfer for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_transfer_create_dto: OpenapiClient::AssetTransferCreateDto.new # AssetTransferCreateDto | 
}

begin
  # Creates a new asset transfer
  result = api_instance.create_asset_transfer_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->create_asset_transfer_async: #{e}"
end
```

#### Using the create_asset_transfer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_asset_transfer_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new asset transfer
  data, status_code, headers = api_instance.create_asset_transfer_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->create_asset_transfer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **asset_transfer_create_dto** | [**AssetTransferCreateDto**](AssetTransferCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_asset_transfer_async

> <EmptyEnvelope> delete_asset_transfer_async(tenant_id, transfer_id)

Deletes an asset transfer

Deletes an asset transfer for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes an asset transfer
  result = api_instance.delete_asset_transfer_async(tenant_id, transfer_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->delete_asset_transfer_async: #{e}"
end
```

#### Using the delete_asset_transfer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_asset_transfer_async_with_http_info(tenant_id, transfer_id)

```ruby
begin
  # Deletes an asset transfer
  data, status_code, headers = api_instance.delete_asset_transfer_async_with_http_info(tenant_id, transfer_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->delete_asset_transfer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_transfer_async

> <AssetTransferDtoEnvelope> get_asset_transfer_async(tenant_id, transfer_id)

Gets a single asset transfer by ID

Retrieves a specific asset transfer by its ID for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a single asset transfer by ID
  result = api_instance.get_asset_transfer_async(tenant_id, transfer_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->get_asset_transfer_async: #{e}"
end
```

#### Using the get_asset_transfer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTransferDtoEnvelope>, Integer, Hash)> get_asset_transfer_async_with_http_info(tenant_id, transfer_id)

```ruby
begin
  # Gets a single asset transfer by ID
  data, status_code, headers = api_instance.get_asset_transfer_async_with_http_info(tenant_id, transfer_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTransferDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->get_asset_transfer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |

### Return type

[**AssetTransferDtoEnvelope**](AssetTransferDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_transfers_async

> <AssetTransferDtoListEnvelope> get_asset_transfers_async(tenant_id)

Gets a list of asset transfers

Retrieves all asset transfers for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a list of asset transfers
  result = api_instance.get_asset_transfers_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->get_asset_transfers_async: #{e}"
end
```

#### Using the get_asset_transfers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AssetTransferDtoListEnvelope>, Integer, Hash)> get_asset_transfers_async_with_http_info(tenant_id)

```ruby
begin
  # Gets a list of asset transfers
  data, status_code, headers = api_instance.get_asset_transfers_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AssetTransferDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->get_asset_transfers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**AssetTransferDtoListEnvelope**](AssetTransferDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_asset_transfers_count_async

> <Int32Envelope> get_asset_transfers_count_async(tenant_id)

Gets the count of asset transfers

Returns the total number of asset transfers for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets the count of asset transfers
  result = api_instance.get_asset_transfers_count_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->get_asset_transfers_count_async: #{e}"
end
```

#### Using the get_asset_transfers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_asset_transfers_count_async_with_http_info(tenant_id)

```ruby
begin
  # Gets the count of asset transfers
  data, status_code, headers = api_instance.get_asset_transfers_count_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->get_asset_transfers_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## patch_asset_transfer_async

> <EmptyEnvelope> patch_asset_transfer_async(tenant_id, transfer_id, opts)

Partially updates an existing asset transfer

Applies a JSON Patch document to an existing asset transfer for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Partially updates an existing asset transfer
  result = api_instance.patch_asset_transfer_async(tenant_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->patch_asset_transfer_async: #{e}"
end
```

#### Using the patch_asset_transfer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_asset_transfer_async_with_http_info(tenant_id, transfer_id, opts)

```ruby
begin
  # Partially updates an existing asset transfer
  data, status_code, headers = api_instance.patch_asset_transfer_async_with_http_info(tenant_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->patch_asset_transfer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_asset_transfer_async

> <EmptyEnvelope> update_asset_transfer_async(tenant_id, transfer_id, opts)

Updates an existing asset transfer

Updates an existing asset transfer for the authenticated tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AssetTransfersApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
transfer_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  asset_transfer_update_dto: OpenapiClient::AssetTransferUpdateDto.new # AssetTransferUpdateDto | 
}

begin
  # Updates an existing asset transfer
  result = api_instance.update_asset_transfer_async(tenant_id, transfer_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->update_asset_transfer_async: #{e}"
end
```

#### Using the update_asset_transfer_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_asset_transfer_async_with_http_info(tenant_id, transfer_id, opts)

```ruby
begin
  # Updates an existing asset transfer
  data, status_code, headers = api_instance.update_asset_transfer_async_with_http_info(tenant_id, transfer_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AssetTransfersApi->update_asset_transfer_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **transfer_id** | **String** |  |  |
| **asset_transfer_update_dto** | [**AssetTransferUpdateDto**](AssetTransferUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

