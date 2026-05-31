# OpenapiClient::ExchangeApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**exchange_amount_async**](ExchangeApi.md#exchange_amount_async) | **GET** /api/v2/ForexService/Exchange/Latest | Exchange currency at latest rates |
| [**exchange_amount_historical_async**](ExchangeApi.md#exchange_amount_historical_async) | **GET** /api/v2/ForexService/Exchange/History | Exchange currency at historical rates |


## exchange_amount_async

> <MoneyEnvelope> exchange_amount_async(amount, source_currency_id, target_currency_id)

Exchange currency at latest rates

Exchange an amount of money from one currency to another using the latest available exchange rates.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExchangeApi.new
amount = 1.2 # Float | 
source_currency_id = 'source_currency_id_example' # String | 
target_currency_id = 'target_currency_id_example' # String | 

begin
  # Exchange currency at latest rates
  result = api_instance.exchange_amount_async(amount, source_currency_id, target_currency_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeApi->exchange_amount_async: #{e}"
end
```

#### Using the exchange_amount_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> exchange_amount_async_with_http_info(amount, source_currency_id, target_currency_id)

```ruby
begin
  # Exchange currency at latest rates
  data, status_code, headers = api_instance.exchange_amount_async_with_http_info(amount, source_currency_id, target_currency_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeApi->exchange_amount_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **amount** | **Float** |  |  |
| **source_currency_id** | **String** |  |  |
| **target_currency_id** | **String** |  |  |

### Return type

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## exchange_amount_historical_async

> <MoneyEnvelope> exchange_amount_historical_async(amount, source_currency_id, target_currency_id, date)

Exchange currency at historical rates

Exchange an amount of money from one currency to another using exchange rates from a specific historical date.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ExchangeApi.new
amount = 1.2 # Float | 
source_currency_id = 'source_currency_id_example' # String | 
target_currency_id = 'target_currency_id_example' # String | 
date = Date.parse('2013-10-20') # Date | 

begin
  # Exchange currency at historical rates
  result = api_instance.exchange_amount_historical_async(amount, source_currency_id, target_currency_id, date)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeApi->exchange_amount_historical_async: #{e}"
end
```

#### Using the exchange_amount_historical_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MoneyEnvelope>, Integer, Hash)> exchange_amount_historical_async_with_http_info(amount, source_currency_id, target_currency_id, date)

```ruby
begin
  # Exchange currency at historical rates
  data, status_code, headers = api_instance.exchange_amount_historical_async_with_http_info(amount, source_currency_id, target_currency_id, date)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MoneyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling ExchangeApi->exchange_amount_historical_async_with_http_info: #{e}"
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

[**MoneyEnvelope**](MoneyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

