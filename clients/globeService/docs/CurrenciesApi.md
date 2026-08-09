# OpenapiClient::CurrenciesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**count_currencies_async**](CurrenciesApi.md#count_currencies_async) | **GET** /api/v2/GlobeService/Currencies/Count | Count currencies |
| [**get_currency_by_id_async**](CurrenciesApi.md#get_currency_by_id_async) | **GET** /api/v2/GlobeService/Currencies/{currencyId} | Get currency by ID |
| [**get_enabled_currencies_async**](CurrenciesApi.md#get_enabled_currencies_async) | **GET** /api/v2/GlobeService/Currencies | Get all currencies |


## count_currencies_async

> <Int32Envelope> count_currencies_async(opts)

Count currencies

Returns the total number of enabled currencies, with optional OData filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurrenciesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  currency_dto_collection_query_parameters: OpenapiClient::CurrencyDtoCollectionQueryParameters.new # CurrencyDtoCollectionQueryParameters | 
}

begin
  # Count currencies
  result = api_instance.count_currencies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurrenciesApi->count_currencies_async: #{e}"
end
```

#### Using the count_currencies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> count_currencies_async_with_http_info(opts)

```ruby
begin
  # Count currencies
  data, status_code, headers = api_instance.count_currencies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurrenciesApi->count_currencies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **currency_dto_collection_query_parameters** | [**CurrencyDtoCollectionQueryParameters**](CurrencyDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_currency_by_id_async

> <CurrencyDtoEnvelope> get_currency_by_id_async(currency_id, opts)

Get currency by ID

Retrieves a single currency by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurrenciesApi.new
currency_id = 'currency_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get currency by ID
  result = api_instance.get_currency_by_id_async(currency_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurrenciesApi->get_currency_by_id_async: #{e}"
end
```

#### Using the get_currency_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurrencyDtoEnvelope>, Integer, Hash)> get_currency_by_id_async_with_http_info(currency_id, opts)

```ruby
begin
  # Get currency by ID
  data, status_code, headers = api_instance.get_currency_by_id_async_with_http_info(currency_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurrencyDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurrenciesApi->get_currency_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **currency_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CurrencyDtoEnvelope**](CurrencyDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_enabled_currencies_async

> <CurrencyDtoListEnvelope> get_enabled_currencies_async(opts)

Get all currencies

Retrieves the list of all enabled currencies with optional OData pagination and filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CurrenciesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  currency_dto_collection_query_parameters: OpenapiClient::CurrencyDtoCollectionQueryParameters.new # CurrencyDtoCollectionQueryParameters | 
}

begin
  # Get all currencies
  result = api_instance.get_enabled_currencies_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurrenciesApi->get_enabled_currencies_async: #{e}"
end
```

#### Using the get_enabled_currencies_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CurrencyDtoListEnvelope>, Integer, Hash)> get_enabled_currencies_async_with_http_info(opts)

```ruby
begin
  # Get all currencies
  data, status_code, headers = api_instance.get_enabled_currencies_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CurrencyDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CurrenciesApi->get_enabled_currencies_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **currency_dto_collection_query_parameters** | [**CurrencyDtoCollectionQueryParameters**](CurrencyDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**CurrencyDtoListEnvelope**](CurrencyDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

