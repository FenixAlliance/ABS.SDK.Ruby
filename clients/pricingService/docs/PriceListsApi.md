# OpenapiClient::PriceListsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_price_list_async**](PriceListsApi.md#create_price_list_async) | **POST** /api/v2/PricingService/PriceLists | Creates a new price list |
| [**create_price_list_prices_async**](PriceListsApi.md#create_price_list_prices_async) | **POST** /api/v2/PricingService/PriceLists/{priceListId}/Prices | Creates a price list entry |
| [**delete_price_list_async**](PriceListsApi.md#delete_price_list_async) | **DELETE** /api/v2/PricingService/PriceLists/{priceListId} | Deletes a price list |
| [**delete_price_list_price_async**](PriceListsApi.md#delete_price_list_price_async) | **DELETE** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Deletes a price list entry |
| [**get_price_list_async**](PriceListsApi.md#get_price_list_async) | **GET** /api/v2/PricingService/PriceLists/{priceListId} | Gets a price list by ID |
| [**get_price_list_price_async**](PriceListsApi.md#get_price_list_price_async) | **GET** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Gets a price list entry by ID |
| [**get_price_list_prices_async**](PriceListsApi.md#get_price_list_prices_async) | **GET** /api/v2/PricingService/PriceLists/{priceListId}/Prices | Retrieves prices in a price list |
| [**get_price_lists_async**](PriceListsApi.md#get_price_lists_async) | **GET** /api/v2/PricingService/PriceLists | Retrieves all price lists |
| [**get_price_lists_count_async**](PriceListsApi.md#get_price_lists_count_async) | **GET** /api/v2/PricingService/PriceLists/Count | Counts price lists |
| [**patch_price_list_async**](PriceListsApi.md#patch_price_list_async) | **PATCH** /api/v2/PricingService/PriceLists/{priceListId} | Patches a price list |
| [**patch_price_list_price_async**](PriceListsApi.md#patch_price_list_price_async) | **PATCH** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Patches a price list entry |
| [**update_price_list_async**](PriceListsApi.md#update_price_list_async) | **PUT** /api/v2/PricingService/PriceLists/{priceListId} | Updates a price list |
| [**update_price_list_price_async**](PriceListsApi.md#update_price_list_price_async) | **PUT** /api/v2/PricingService/PriceLists/{priceListId}/Prices/{priceId} | Updates a price list entry |


## create_price_list_async

> <EmptyEnvelope> create_price_list_async(tenant_id, opts)

Creates a new price list

Creates a new price list for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  price_list_create_dto: OpenapiClient::PriceListCreateDto.new({name: 'name_example'}) # PriceListCreateDto | 
}

begin
  # Creates a new price list
  result = api_instance.create_price_list_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->create_price_list_async: #{e}"
end
```

#### Using the create_price_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_price_list_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Creates a new price list
  data, status_code, headers = api_instance.create_price_list_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->create_price_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_create_dto** | [**PriceListCreateDto**](PriceListCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## create_price_list_prices_async

> <EmptyEnvelope> create_price_list_prices_async(tenant_id, price_list_id, opts)

Creates a price list entry

Creates a new price entry in the specified price list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_price_create_dto: OpenapiClient::ItemPriceCreateDto.new({item_id: 'item_id_example'}) # ItemPriceCreateDto | 
}

begin
  # Creates a price list entry
  result = api_instance.create_price_list_prices_async(tenant_id, price_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->create_price_list_prices_async: #{e}"
end
```

#### Using the create_price_list_prices_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_price_list_prices_async_with_http_info(tenant_id, price_list_id, opts)

```ruby
begin
  # Creates a price list entry
  data, status_code, headers = api_instance.create_price_list_prices_async_with_http_info(tenant_id, price_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->create_price_list_prices_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **item_price_create_dto** | [**ItemPriceCreateDto**](ItemPriceCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_price_list_async

> <EmptyEnvelope> delete_price_list_async(tenant_id, price_list_id)

Deletes a price list

Deletes the specified price list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a price list
  result = api_instance.delete_price_list_async(tenant_id, price_list_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->delete_price_list_async: #{e}"
end
```

#### Using the delete_price_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_price_list_async_with_http_info(tenant_id, price_list_id)

```ruby
begin
  # Deletes a price list
  data, status_code, headers = api_instance.delete_price_list_async_with_http_info(tenant_id, price_list_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->delete_price_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## delete_price_list_price_async

> <EmptyEnvelope> delete_price_list_price_async(tenant_id, price_list_id, price_id)

Deletes a price list entry

Deletes the specified price entry from a price list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Deletes a price list entry
  result = api_instance.delete_price_list_price_async(tenant_id, price_list_id, price_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->delete_price_list_price_async: #{e}"
end
```

#### Using the delete_price_list_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id)

```ruby
begin
  # Deletes a price list entry
  data, status_code, headers = api_instance.delete_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->delete_price_list_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **price_id** | **String** |  |  |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_price_list_async

> <PriceListDtoEnvelope> get_price_list_async(tenant_id, price_list_id)

Gets a price list by ID

Retrieves the details of a price list using its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a price list by ID
  result = api_instance.get_price_list_async(tenant_id, price_list_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_list_async: #{e}"
end
```

#### Using the get_price_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PriceListDtoEnvelope>, Integer, Hash)> get_price_list_async_with_http_info(tenant_id, price_list_id)

```ruby
begin
  # Gets a price list by ID
  data, status_code, headers = api_instance.get_price_list_async_with_http_info(tenant_id, price_list_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PriceListDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |

### Return type

[**PriceListDtoEnvelope**](PriceListDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_price_list_price_async

> <ItemPriceDtoEnvelope> get_price_list_price_async(tenant_id, price_list_id, price_id)

Gets a price list entry by ID

Retrieves a specific price entry from a price list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Gets a price list entry by ID
  result = api_instance.get_price_list_price_async(tenant_id, price_list_id, price_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_list_price_async: #{e}"
end
```

#### Using the get_price_list_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPriceDtoEnvelope>, Integer, Hash)> get_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id)

```ruby
begin
  # Gets a price list entry by ID
  data, status_code, headers = api_instance.get_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPriceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_list_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **price_id** | **String** |  |  |

### Return type

[**ItemPriceDtoEnvelope**](ItemPriceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_price_list_prices_async

> <ItemPriceDtoListEnvelope> get_price_list_prices_async(tenant_id, price_list_id, opts)

Retrieves prices in a price list

Gets all price entries for a specific price list with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_id: '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
}

begin
  # Retrieves prices in a price list
  result = api_instance.get_price_list_prices_async(tenant_id, price_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_list_prices_async: #{e}"
end
```

#### Using the get_price_list_prices_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemPriceDtoListEnvelope>, Integer, Hash)> get_price_list_prices_async_with_http_info(tenant_id, price_list_id, opts)

```ruby
begin
  # Retrieves prices in a price list
  data, status_code, headers = api_instance.get_price_list_prices_async_with_http_info(tenant_id, price_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemPriceDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_list_prices_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **item_id** | **String** |  | [optional] |

### Return type

[**ItemPriceDtoListEnvelope**](ItemPriceDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_price_lists_async

> <PriceListDtoListEnvelope> get_price_lists_async(tenant_id)

Retrieves all price lists

Gets all price lists for the current tenant with OData support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Retrieves all price lists
  result = api_instance.get_price_lists_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_lists_async: #{e}"
end
```

#### Using the get_price_lists_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PriceListDtoListEnvelope>, Integer, Hash)> get_price_lists_async_with_http_info(tenant_id)

```ruby
begin
  # Retrieves all price lists
  data, status_code, headers = api_instance.get_price_lists_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PriceListDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_lists_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |

### Return type

[**PriceListDtoListEnvelope**](PriceListDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_price_lists_count_async

> <Int32Envelope> get_price_lists_count_async(tenant_id)

Counts price lists

Gets the count of price lists for the current tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Counts price lists
  result = api_instance.get_price_lists_count_async(tenant_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_lists_count_async: #{e}"
end
```

#### Using the get_price_lists_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_price_lists_count_async_with_http_info(tenant_id)

```ruby
begin
  # Counts price lists
  data, status_code, headers = api_instance.get_price_lists_count_async_with_http_info(tenant_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->get_price_lists_count_async_with_http_info: #{e}"
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


## patch_price_list_async

> <EmptyEnvelope> patch_price_list_async(tenant_id, price_list_id, opts)

Patches a price list

Partially updates the specified price list using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a price list
  result = api_instance.patch_price_list_async(tenant_id, price_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->patch_price_list_async: #{e}"
end
```

#### Using the patch_price_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_price_list_async_with_http_info(tenant_id, price_list_id, opts)

```ruby
begin
  # Patches a price list
  data, status_code, headers = api_instance.patch_price_list_async_with_http_info(tenant_id, price_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->patch_price_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_price_list_price_async

> <EmptyEnvelope> patch_price_list_price_async(tenant_id, price_list_id, price_id, opts)

Patches a price list entry

Partially updates the specified price entry in a price list using a JSON Patch document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patches a price list entry
  result = api_instance.patch_price_list_price_async(tenant_id, price_list_id, price_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->patch_price_list_price_async: #{e}"
end
```

#### Using the patch_price_list_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id, opts)

```ruby
begin
  # Patches a price list entry
  data, status_code, headers = api_instance.patch_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->patch_price_list_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **price_id** | **String** |  |  |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_price_list_async

> <EmptyEnvelope> update_price_list_async(tenant_id, price_list_id, opts)

Updates a price list

Updates the specified price list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  price_list_update_dto: OpenapiClient::PriceListUpdateDto.new({name: 'name_example'}) # PriceListUpdateDto | 
}

begin
  # Updates a price list
  result = api_instance.update_price_list_async(tenant_id, price_list_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->update_price_list_async: #{e}"
end
```

#### Using the update_price_list_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_price_list_async_with_http_info(tenant_id, price_list_id, opts)

```ruby
begin
  # Updates a price list
  data, status_code, headers = api_instance.update_price_list_async_with_http_info(tenant_id, price_list_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->update_price_list_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **price_list_update_dto** | [**PriceListUpdateDto**](PriceListUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_price_list_price_async

> <EmptyEnvelope> update_price_list_price_async(tenant_id, price_list_id, price_id, opts)

Updates a price list entry

Updates the specified price entry in a price list.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::PriceListsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_list_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
price_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  item_price_update_dto: OpenapiClient::ItemPriceUpdateDto.new # ItemPriceUpdateDto | 
}

begin
  # Updates a price list entry
  result = api_instance.update_price_list_price_async(tenant_id, price_list_id, price_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->update_price_list_price_async: #{e}"
end
```

#### Using the update_price_list_price_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id, opts)

```ruby
begin
  # Updates a price list entry
  data, status_code, headers = api_instance.update_price_list_price_async_with_http_info(tenant_id, price_list_id, price_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling PriceListsApi->update_price_list_price_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **price_list_id** | **String** |  |  |
| **price_id** | **String** |  |  |
| **item_price_update_dto** | [**ItemPriceUpdateDto**](ItemPriceUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

