# OpenapiClient::ExchangeVApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**exchange_amount_historical_v3_async**](ExchangeVApi.md#exchange_amount_historical_v3_async) | **GET** /api/v3/ForexService/Exchange/History | Exchange currency at historical rates (v3) |
| [**exchange_amount_v3_async**](ExchangeVApi.md#exchange_amount_v3_async) | **GET** /api/v3/ForexService/Exchange/Latest | Exchange currency at latest rates (v3) |


## exchange_amount_historical_v3_async

> <ExchangeRateEnvelope> exchange_amount_historical_v3_async(amount, source_currency_id, target_currency_id, date)

Exchange currency at historical rates (v3)

Exchange an amount of money from one currency to another using exchange rates from a specific historical date. Returns the full ExchangeRate details.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExchangeVApi.new
amount = 1.2 # Float | 
source_currency_id = 'source_currency_id_example' # String | 
target_currency_id = 'target_currency_id_example' # String | 
date = Date.parse('2013-10-20') # Date | 

begin
  # Exchange currency at historical rates (v3)
  result = api_instance.exchange_amount_historical_v3_async(amount, source_currency_id, target_currency_id, date)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeVApi->exchange_amount_historical_v3_async: #{e}"
end
```

#### Using the exchange_amount_historical_v3_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExchangeRateEnvelope>, Integer, Hash)> exchange_amount_historical_v3_async_with_http_info(amount, source_currency_id, target_currency_id, date)

```ruby
begin
  # Exchange currency at historical rates (v3)
  data, status_code, headers = api_instance.exchange_amount_historical_v3_async_with_http_info(amount, source_currency_id, target_currency_id, date)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExchangeRateEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeVApi->exchange_amount_historical_v3_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **amount** | **Float** |  |  |
| **source_currency_id** | **String** |  |  |
| **target_currency_id** | **String** |  |  |
| **date** | **Date** |  |  |

### Return type

[**ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## exchange_amount_v3_async

> <ExchangeRateEnvelope> exchange_amount_v3_async(amount, source_currency_id, target_currency_id)

Exchange currency at latest rates (v3)

Exchange an amount of money from one currency to another using the latest available exchange rates. Returns the full ExchangeRate details.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExchangeVApi.new
amount = 1.2 # Float | 
source_currency_id = 'source_currency_id_example' # String | 
target_currency_id = 'target_currency_id_example' # String | 

begin
  # Exchange currency at latest rates (v3)
  result = api_instance.exchange_amount_v3_async(amount, source_currency_id, target_currency_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeVApi->exchange_amount_v3_async: #{e}"
end
```

#### Using the exchange_amount_v3_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExchangeRateEnvelope>, Integer, Hash)> exchange_amount_v3_async_with_http_info(amount, source_currency_id, target_currency_id)

```ruby
begin
  # Exchange currency at latest rates (v3)
  data, status_code, headers = api_instance.exchange_amount_v3_async_with_http_info(amount, source_currency_id, target_currency_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExchangeRateEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeVApi->exchange_amount_v3_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **amount** | **Float** |  |  |
| **source_currency_id** | **String** |  |  |
| **target_currency_id** | **String** |  |  |

### Return type

[**ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

