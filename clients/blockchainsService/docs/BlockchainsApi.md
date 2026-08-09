# OpenapiClient::BlockchainsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_blockchain_async**](BlockchainsApi.md#create_blockchain_async) | **POST** /api/v2/BlockchainsService/Blockchains | Create a new blockchain |
| [**create_blockchain_block_async**](BlockchainsApi.md#create_blockchain_block_async) | **POST** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks | Add a block to a blockchain |
| [**delete_blockchain_async**](BlockchainsApi.md#delete_blockchain_async) | **DELETE** /api/v2/BlockchainsService/Blockchains/{id} | Delete a blockchain |
| [**delete_blockchain_block_async**](BlockchainsApi.md#delete_blockchain_block_async) | **DELETE** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Delete a blockchain block |
| [**get_blockchain_block_by_id_async**](BlockchainsApi.md#get_blockchain_block_by_id_async) | **GET** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Get a specific block |
| [**get_blockchain_blocks_async**](BlockchainsApi.md#get_blockchain_blocks_async) | **GET** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks | Get blocks for a blockchain |
| [**get_blockchain_blocks_count_async**](BlockchainsApi.md#get_blockchain_blocks_count_async) | **GET** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/Count | Get block count for a blockchain |
| [**get_blockchain_by_id_async**](BlockchainsApi.md#get_blockchain_by_id_async) | **GET** /api/v2/BlockchainsService/Blockchains/{id} | Get blockchain by ID |
| [**get_blockchains_async**](BlockchainsApi.md#get_blockchains_async) | **GET** /api/v2/BlockchainsService/Blockchains | Get all blockchains |
| [**get_blockchains_count_async**](BlockchainsApi.md#get_blockchains_count_async) | **GET** /api/v2/BlockchainsService/Blockchains/Count | Get blockchains count |
| [**patch_blockchain_async**](BlockchainsApi.md#patch_blockchain_async) | **PATCH** /api/v2/BlockchainsService/Blockchains/{id} | Patch a blockchain |
| [**patch_blockchain_block_async**](BlockchainsApi.md#patch_blockchain_block_async) | **PATCH** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Patch a blockchain block |
| [**update_blockchain_async**](BlockchainsApi.md#update_blockchain_async) | **PUT** /api/v2/BlockchainsService/Blockchains/{id} | Update a blockchain |
| [**update_blockchain_block_async**](BlockchainsApi.md#update_blockchain_block_async) | **PUT** /api/v2/BlockchainsService/Blockchains/{blockchainId}/Blocks/{blockId} | Update a blockchain block |


## create_blockchain_async

> create_blockchain_async(tenant_id, opts)

Create a new blockchain

Creates a new blockchain for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_create_dto: OpenapiClient::BlockchainCreateDto.new({name: 'name_example'}) # BlockchainCreateDto | 
}

begin
  # Create a new blockchain
  api_instance.create_blockchain_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->create_blockchain_async: #{e}"
end
```

#### Using the create_blockchain_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_blockchain_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new blockchain
  data, status_code, headers = api_instance.create_blockchain_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->create_blockchain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_create_dto** | [**BlockchainCreateDto**](BlockchainCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_blockchain_block_async

> create_blockchain_block_async(tenant_id, blockchain_id, opts)

Add a block to a blockchain

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_block_create_dto: OpenapiClient::BlockchainBlockCreateDto.new({hash: 'hash_example', blockchain_id: 'blockchain_id_example', wallet_account_id: 'wallet_account_id_example'}) # BlockchainBlockCreateDto | 
}

begin
  # Add a block to a blockchain
  api_instance.create_blockchain_block_async(tenant_id, blockchain_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->create_blockchain_block_async: #{e}"
end
```

#### Using the create_blockchain_block_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_blockchain_block_async_with_http_info(tenant_id, blockchain_id, opts)

```ruby
begin
  # Add a block to a blockchain
  data, status_code, headers = api_instance.create_blockchain_block_async_with_http_info(tenant_id, blockchain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->create_blockchain_block_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_block_create_dto** | [**BlockchainBlockCreateDto**](BlockchainBlockCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined


## delete_blockchain_async

> delete_blockchain_async(tenant_id, id, opts)

Delete a blockchain

Deletes a blockchain for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a blockchain
  api_instance.delete_blockchain_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->delete_blockchain_async: #{e}"
end
```

#### Using the delete_blockchain_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_blockchain_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a blockchain
  data, status_code, headers = api_instance.delete_blockchain_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->delete_blockchain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_blockchain_block_async

> delete_blockchain_block_async(tenant_id, blockchain_id, block_id, opts)

Delete a blockchain block

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
block_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a blockchain block
  api_instance.delete_blockchain_block_async(tenant_id, blockchain_id, block_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->delete_blockchain_block_async: #{e}"
end
```

#### Using the delete_blockchain_block_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_blockchain_block_async_with_http_info(tenant_id, blockchain_id, block_id, opts)

```ruby
begin
  # Delete a blockchain block
  data, status_code, headers = api_instance.delete_blockchain_block_async_with_http_info(tenant_id, blockchain_id, block_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->delete_blockchain_block_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **block_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## get_blockchain_block_by_id_async

> <BlockchainBlockDto> get_blockchain_block_by_id_async(tenant_id, blockchain_id, block_id, opts)

Get a specific block

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
block_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a specific block
  result = api_instance.get_blockchain_block_by_id_async(tenant_id, blockchain_id, block_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_block_by_id_async: #{e}"
end
```

#### Using the get_blockchain_block_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlockchainBlockDto>, Integer, Hash)> get_blockchain_block_by_id_async_with_http_info(tenant_id, blockchain_id, block_id, opts)

```ruby
begin
  # Get a specific block
  data, status_code, headers = api_instance.get_blockchain_block_by_id_async_with_http_info(tenant_id, blockchain_id, block_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlockchainBlockDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_block_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **block_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlockchainBlockDto**](BlockchainBlockDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blockchain_blocks_async

> <BlockchainBlockDtoListEnvelope> get_blockchain_blocks_async(tenant_id, blockchain_id, opts)

Get blocks for a blockchain

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_block_dto_collection_query_parameters: OpenapiClient::BlockchainBlockDtoCollectionQueryParameters.new # BlockchainBlockDtoCollectionQueryParameters | 
}

begin
  # Get blocks for a blockchain
  result = api_instance.get_blockchain_blocks_async(tenant_id, blockchain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_blocks_async: #{e}"
end
```

#### Using the get_blockchain_blocks_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlockchainBlockDtoListEnvelope>, Integer, Hash)> get_blockchain_blocks_async_with_http_info(tenant_id, blockchain_id, opts)

```ruby
begin
  # Get blocks for a blockchain
  data, status_code, headers = api_instance.get_blockchain_blocks_async_with_http_info(tenant_id, blockchain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlockchainBlockDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_blocks_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_block_dto_collection_query_parameters** | [**BlockchainBlockDtoCollectionQueryParameters**](BlockchainBlockDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BlockchainBlockDtoListEnvelope**](BlockchainBlockDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_blockchain_blocks_count_async

> <Int32Envelope> get_blockchain_blocks_count_async(tenant_id, blockchain_id, opts)

Get block count for a blockchain

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_block_dto_collection_query_parameters: OpenapiClient::BlockchainBlockDtoCollectionQueryParameters.new # BlockchainBlockDtoCollectionQueryParameters | 
}

begin
  # Get block count for a blockchain
  result = api_instance.get_blockchain_blocks_count_async(tenant_id, blockchain_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_blocks_count_async: #{e}"
end
```

#### Using the get_blockchain_blocks_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_blockchain_blocks_count_async_with_http_info(tenant_id, blockchain_id, opts)

```ruby
begin
  # Get block count for a blockchain
  data, status_code, headers = api_instance.get_blockchain_blocks_count_async_with_http_info(tenant_id, blockchain_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_blocks_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_block_dto_collection_query_parameters** | [**BlockchainBlockDtoCollectionQueryParameters**](BlockchainBlockDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_blockchain_by_id_async

> <BlockchainDto> get_blockchain_by_id_async(tenant_id, id, opts)

Get blockchain by ID

Retrieves a specific blockchain by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get blockchain by ID
  result = api_instance.get_blockchain_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_by_id_async: #{e}"
end
```

#### Using the get_blockchain_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlockchainDto>, Integer, Hash)> get_blockchain_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get blockchain by ID
  data, status_code, headers = api_instance.get_blockchain_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlockchainDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchain_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BlockchainDto**](BlockchainDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_blockchains_async

> <BlockchainDtoListEnvelope> get_blockchains_async(tenant_id, opts)

Get all blockchains

Retrieves all blockchains for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_dto_collection_query_parameters: OpenapiClient::BlockchainDtoCollectionQueryParameters.new # BlockchainDtoCollectionQueryParameters | 
}

begin
  # Get all blockchains
  result = api_instance.get_blockchains_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchains_async: #{e}"
end
```

#### Using the get_blockchains_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BlockchainDtoListEnvelope>, Integer, Hash)> get_blockchains_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all blockchains
  data, status_code, headers = api_instance.get_blockchains_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BlockchainDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchains_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_dto_collection_query_parameters** | [**BlockchainDtoCollectionQueryParameters**](BlockchainDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**BlockchainDtoListEnvelope**](BlockchainDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_blockchains_count_async

> <Int32Envelope> get_blockchains_count_async(tenant_id, opts)

Get blockchains count

Returns the count of blockchains for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_dto_collection_query_parameters: OpenapiClient::BlockchainDtoCollectionQueryParameters.new # BlockchainDtoCollectionQueryParameters | 
}

begin
  # Get blockchains count
  result = api_instance.get_blockchains_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchains_count_async: #{e}"
end
```

#### Using the get_blockchains_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_blockchains_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get blockchains count
  data, status_code, headers = api_instance.get_blockchains_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->get_blockchains_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_dto_collection_query_parameters** | [**BlockchainDtoCollectionQueryParameters**](BlockchainDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_blockchain_async

> <EmptyEnvelope> patch_blockchain_async(tenant_id, id, opts)

Patch a blockchain

Patch a blockchain

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a blockchain
  result = api_instance.patch_blockchain_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->patch_blockchain_async: #{e}"
end
```

#### Using the patch_blockchain_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_blockchain_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a blockchain
  data, status_code, headers = api_instance.patch_blockchain_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->patch_blockchain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
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


## patch_blockchain_block_async

> <EmptyEnvelope> patch_blockchain_block_async(tenant_id, blockchain_id, block_id, opts)

Patch a blockchain block

Patch a blockchain block

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
block_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a blockchain block
  result = api_instance.patch_blockchain_block_async(tenant_id, blockchain_id, block_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->patch_blockchain_block_async: #{e}"
end
```

#### Using the patch_blockchain_block_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_blockchain_block_async_with_http_info(tenant_id, blockchain_id, block_id, opts)

```ruby
begin
  # Patch a blockchain block
  data, status_code, headers = api_instance.patch_blockchain_block_async_with_http_info(tenant_id, blockchain_id, block_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->patch_blockchain_block_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **block_id** | **String** |  |  |
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


## update_blockchain_async

> update_blockchain_async(tenant_id, id, opts)

Update a blockchain

Updates an existing blockchain for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_update_dto: OpenapiClient::BlockchainUpdateDto.new # BlockchainUpdateDto | 
}

begin
  # Update a blockchain
  api_instance.update_blockchain_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->update_blockchain_async: #{e}"
end
```

#### Using the update_blockchain_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_blockchain_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a blockchain
  data, status_code, headers = api_instance.update_blockchain_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->update_blockchain_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_update_dto** | [**BlockchainUpdateDto**](BlockchainUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_blockchain_block_async

> update_blockchain_block_async(tenant_id, blockchain_id, block_id, opts)

Update a blockchain block

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::BlockchainsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
blockchain_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
block_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  blockchain_block_update_dto: OpenapiClient::BlockchainBlockUpdateDto.new # BlockchainBlockUpdateDto | 
}

begin
  # Update a blockchain block
  api_instance.update_blockchain_block_async(tenant_id, blockchain_id, block_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->update_blockchain_block_async: #{e}"
end
```

#### Using the update_blockchain_block_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_blockchain_block_async_with_http_info(tenant_id, blockchain_id, block_id, opts)

```ruby
begin
  # Update a blockchain block
  data, status_code, headers = api_instance.update_blockchain_block_async_with_http_info(tenant_id, blockchain_id, block_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling BlockchainsApi->update_blockchain_block_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **blockchain_id** | **String** |  |  |
| **block_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **blockchain_block_update_dto** | [**BlockchainBlockUpdateDto**](BlockchainBlockUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: Not defined

