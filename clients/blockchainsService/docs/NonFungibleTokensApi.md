# OpenapiClient::NonFungibleTokensApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_non_fungible_token_async**](NonFungibleTokensApi.md#create_non_fungible_token_async) | **POST** /api/v2/BlockchainsService/NonFungibleTokens | Create a new NFT |
| [**delete_non_fungible_token_async**](NonFungibleTokensApi.md#delete_non_fungible_token_async) | **DELETE** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Delete an NFT |
| [**get_non_fungible_token_by_id_async**](NonFungibleTokensApi.md#get_non_fungible_token_by_id_async) | **GET** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Get NFT by ID |
| [**get_non_fungible_tokens_async**](NonFungibleTokensApi.md#get_non_fungible_tokens_async) | **GET** /api/v2/BlockchainsService/NonFungibleTokens | Get all non-fungible tokens |
| [**get_non_fungible_tokens_count_async**](NonFungibleTokensApi.md#get_non_fungible_tokens_count_async) | **GET** /api/v2/BlockchainsService/NonFungibleTokens/Count | Get NFTs count |
| [**patch_non_fungible_token_async**](NonFungibleTokensApi.md#patch_non_fungible_token_async) | **PATCH** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Patch a non-fungible token |
| [**update_non_fungible_token_async**](NonFungibleTokensApi.md#update_non_fungible_token_async) | **PUT** /api/v2/BlockchainsService/NonFungibleTokens/{id} | Update an NFT |


## create_non_fungible_token_async

> create_non_fungible_token_async(tenant_id, opts)

Create a new NFT

Creates a new non-fungible token for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  non_fungible_token_create_dto: OpenapiClient::NonFungibleTokenCreateDto.new({title: 'title_example', description: 'description_example'}) # NonFungibleTokenCreateDto | 
}

begin
  # Create a new NFT
  api_instance.create_non_fungible_token_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->create_non_fungible_token_async: #{e}"
end
```

#### Using the create_non_fungible_token_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_non_fungible_token_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new NFT
  data, status_code, headers = api_instance.create_non_fungible_token_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->create_non_fungible_token_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **non_fungible_token_create_dto** | [**NonFungibleTokenCreateDto**](NonFungibleTokenCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_non_fungible_token_async

> delete_non_fungible_token_async(tenant_id, id, opts)

Delete an NFT

Deletes a non-fungible token for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete an NFT
  api_instance.delete_non_fungible_token_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->delete_non_fungible_token_async: #{e}"
end
```

#### Using the delete_non_fungible_token_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_non_fungible_token_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete an NFT
  data, status_code, headers = api_instance.delete_non_fungible_token_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->delete_non_fungible_token_async_with_http_info: #{e}"
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


## get_non_fungible_token_by_id_async

> <NonFungibleTokenDto> get_non_fungible_token_by_id_async(tenant_id, id, opts)

Get NFT by ID

Retrieves a specific non-fungible token by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get NFT by ID
  result = api_instance.get_non_fungible_token_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->get_non_fungible_token_by_id_async: #{e}"
end
```

#### Using the get_non_fungible_token_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NonFungibleTokenDto>, Integer, Hash)> get_non_fungible_token_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get NFT by ID
  data, status_code, headers = api_instance.get_non_fungible_token_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NonFungibleTokenDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->get_non_fungible_token_by_id_async_with_http_info: #{e}"
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

[**NonFungibleTokenDto**](NonFungibleTokenDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_non_fungible_tokens_async

> <NonFungibleTokenDtoListEnvelope> get_non_fungible_tokens_async(tenant_id, opts)

Get all non-fungible tokens

Retrieves all NFTs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  non_fungible_token_dto_collection_query_parameters: OpenapiClient::NonFungibleTokenDtoCollectionQueryParameters.new # NonFungibleTokenDtoCollectionQueryParameters | 
}

begin
  # Get all non-fungible tokens
  result = api_instance.get_non_fungible_tokens_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->get_non_fungible_tokens_async: #{e}"
end
```

#### Using the get_non_fungible_tokens_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<NonFungibleTokenDtoListEnvelope>, Integer, Hash)> get_non_fungible_tokens_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all non-fungible tokens
  data, status_code, headers = api_instance.get_non_fungible_tokens_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <NonFungibleTokenDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->get_non_fungible_tokens_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **non_fungible_token_dto_collection_query_parameters** | [**NonFungibleTokenDtoCollectionQueryParameters**](NonFungibleTokenDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**NonFungibleTokenDtoListEnvelope**](NonFungibleTokenDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_non_fungible_tokens_count_async

> <Int32Envelope> get_non_fungible_tokens_count_async(tenant_id, opts)

Get NFTs count

Returns the count of NFTs for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  non_fungible_token_dto_collection_query_parameters: OpenapiClient::NonFungibleTokenDtoCollectionQueryParameters.new # NonFungibleTokenDtoCollectionQueryParameters | 
}

begin
  # Get NFTs count
  result = api_instance.get_non_fungible_tokens_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->get_non_fungible_tokens_count_async: #{e}"
end
```

#### Using the get_non_fungible_tokens_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_non_fungible_tokens_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get NFTs count
  data, status_code, headers = api_instance.get_non_fungible_tokens_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->get_non_fungible_tokens_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **non_fungible_token_dto_collection_query_parameters** | [**NonFungibleTokenDtoCollectionQueryParameters**](NonFungibleTokenDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_non_fungible_token_async

> <EmptyEnvelope> patch_non_fungible_token_async(tenant_id, id, opts)

Patch a non-fungible token

Patch a non-fungible token

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a non-fungible token
  result = api_instance.patch_non_fungible_token_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->patch_non_fungible_token_async: #{e}"
end
```

#### Using the patch_non_fungible_token_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_non_fungible_token_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a non-fungible token
  data, status_code, headers = api_instance.patch_non_fungible_token_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->patch_non_fungible_token_async_with_http_info: #{e}"
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


## update_non_fungible_token_async

> update_non_fungible_token_async(tenant_id, id, opts)

Update an NFT

Updates an existing non-fungible token for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::NonFungibleTokensApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  non_fungible_token_update_dto: OpenapiClient::NonFungibleTokenUpdateDto.new # NonFungibleTokenUpdateDto | 
}

begin
  # Update an NFT
  api_instance.update_non_fungible_token_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->update_non_fungible_token_async: #{e}"
end
```

#### Using the update_non_fungible_token_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_non_fungible_token_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update an NFT
  data, status_code, headers = api_instance.update_non_fungible_token_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling NonFungibleTokensApi->update_non_fungible_token_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **non_fungible_token_update_dto** | [**NonFungibleTokenUpdateDto**](NonFungibleTokenUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

