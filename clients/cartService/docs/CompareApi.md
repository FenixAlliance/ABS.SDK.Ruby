# OpenapiClient::CompareApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**add_item_to_compare_table_async**](CompareApi.md#add_item_to_compare_table_async) | **POST** /api/v2/CartService/Compare | Add an item to the compare table |
| [**get_item_to_compare_record**](CompareApi.md#get_item_to_compare_record) | **GET** /api/v2/CartService/Compare/{recordId}/Details | Get compare record details |
| [**get_item_to_compare_records**](CompareApi.md#get_item_to_compare_records) | **GET** /api/v2/CartService/Compare/{cartId} | Get items to compare in a cart |
| [**remove_item_from_compare_table**](CompareApi.md#remove_item_from_compare_table) | **DELETE** /api/v2/CartService/Compare/{recordId} | Remove an item from the compare table |


## add_item_to_compare_table_async

> <ItemCartRecordDto> add_item_to_compare_table_async(opts)

Add an item to the compare table

Adds a product to the compare table for the specified cart with tracking.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CompareApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  add_product_to_compare_request: OpenapiClient::AddProductToCompareRequest.new # AddProductToCompareRequest | 
}

begin
  # Add an item to the compare table
  result = api_instance.add_item_to_compare_table_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->add_item_to_compare_table_async: #{e}"
end
```

#### Using the add_item_to_compare_table_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemCartRecordDto>, Integer, Hash)> add_item_to_compare_table_async_with_http_info(opts)

```ruby
begin
  # Add an item to the compare table
  data, status_code, headers = api_instance.add_item_to_compare_table_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemCartRecordDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->add_item_to_compare_table_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **add_product_to_compare_request** | [**AddProductToCompareRequest**](AddProductToCompareRequest.md) |  | [optional] |

### Return type

[**ItemCartRecordDto**](ItemCartRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_item_to_compare_record

> <ItemToCompareCartRecordDtoEnvelope> get_item_to_compare_record(record_id, opts)

Get compare record details

Retrieves the details of a specific item-to-compare cart record.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CompareApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get compare record details
  result = api_instance.get_item_to_compare_record(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->get_item_to_compare_record: #{e}"
end
```

#### Using the get_item_to_compare_record_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemToCompareCartRecordDtoEnvelope>, Integer, Hash)> get_item_to_compare_record_with_http_info(record_id, opts)

```ruby
begin
  # Get compare record details
  data, status_code, headers = api_instance.get_item_to_compare_record_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemToCompareCartRecordDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->get_item_to_compare_record_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemToCompareCartRecordDtoEnvelope**](ItemToCompareCartRecordDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_item_to_compare_records

> <ItemToCompareCartRecordDtoListEnvelope> get_item_to_compare_records(cart_id, opts)

Get items to compare in a cart

Retrieves all items added to the compare table for the specified cart.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CompareApi.new
cart_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get items to compare in a cart
  result = api_instance.get_item_to_compare_records(cart_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->get_item_to_compare_records: #{e}"
end
```

#### Using the get_item_to_compare_records_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemToCompareCartRecordDtoListEnvelope>, Integer, Hash)> get_item_to_compare_records_with_http_info(cart_id, opts)

```ruby
begin
  # Get items to compare in a cart
  data, status_code, headers = api_instance.get_item_to_compare_records_with_http_info(cart_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemToCompareCartRecordDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->get_item_to_compare_records_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **cart_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemToCompareCartRecordDtoListEnvelope**](ItemToCompareCartRecordDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## remove_item_from_compare_table

> <ItemToCompareCartRecordDto> remove_item_from_compare_table(record_id, opts)

Remove an item from the compare table

Removes a specific record from the compare table by its record ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CompareApi.new
record_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Remove an item from the compare table
  result = api_instance.remove_item_from_compare_table(record_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->remove_item_from_compare_table: #{e}"
end
```

#### Using the remove_item_from_compare_table_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ItemToCompareCartRecordDto>, Integer, Hash)> remove_item_from_compare_table_with_http_info(record_id, opts)

```ruby
begin
  # Remove an item from the compare table
  data, status_code, headers = api_instance.remove_item_from_compare_table_with_http_info(record_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ItemToCompareCartRecordDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CompareApi->remove_item_from_compare_table_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **record_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ItemToCompareCartRecordDto**](ItemToCompareCartRecordDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

