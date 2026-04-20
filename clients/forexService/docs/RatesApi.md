# OpenapiClient::RatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_historical_currency_rate_async**](RatesApi.md#get_historical_currency_rate_async) | **GET** /api/v2/ForexService/Rates/History/{currencyId} | Get historical rate for a currency |
| [**get_historical_currency_rates_async**](RatesApi.md#get_historical_currency_rates_async) | **GET** /api/v2/ForexService/Rates/History | Get historical currency rates |
| [**get_latest_currency_rate_async**](RatesApi.md#get_latest_currency_rate_async) | **GET** /api/v2/ForexService/Rates/Latest/{currencyId} | Get latest rate for a currency |
| [**get_latest_currency_rates_model_async**](RatesApi.md#get_latest_currency_rates_model_async) | **GET** /api/v2/ForexService/Rates/Latest | Get latest currency rates |


## get_historical_currency_rate_async

> <ExchangeRateEnvelope> get_historical_currency_rate_async(currency_id, opts)

Get historical rate for a currency

Retrieves the exchange rate for a specific currency as of a specific historical date.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RatesApi.new
currency_id = 'currency_id_example' # String | 
opts = {
  date: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get historical rate for a currency
  result = api_instance.get_historical_currency_rate_async(currency_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_historical_currency_rate_async: #{e}"
end
```

#### Using the get_historical_currency_rate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExchangeRateEnvelope>, Integer, Hash)> get_historical_currency_rate_async_with_http_info(currency_id, opts)

```ruby
begin
  # Get historical rate for a currency
  data, status_code, headers = api_instance.get_historical_currency_rate_async_with_http_info(currency_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExchangeRateEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_historical_currency_rate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **currency_id** | **String** |  |  |
| **date** | **Time** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_historical_currency_rates_async

> <ForexRatesDtoEnvelope> get_historical_currency_rates_async(opts)

Get historical currency rates

Retrieves exchange rates for all supported currencies as of a specific historical date.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RatesApi.new
opts = {
  date: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get historical currency rates
  result = api_instance.get_historical_currency_rates_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_historical_currency_rates_async: #{e}"
end
```

#### Using the get_historical_currency_rates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ForexRatesDtoEnvelope>, Integer, Hash)> get_historical_currency_rates_async_with_http_info(opts)

```ruby
begin
  # Get historical currency rates
  data, status_code, headers = api_instance.get_historical_currency_rates_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ForexRatesDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_historical_currency_rates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **date** | **Time** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ForexRatesDtoEnvelope**](ForexRatesDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_latest_currency_rate_async

> <ExchangeRateEnvelope> get_latest_currency_rate_async(currency_id, opts)

Get latest rate for a currency

Retrieves the latest exchange rate for a specific currency by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RatesApi.new
currency_id = 'currency_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get latest rate for a currency
  result = api_instance.get_latest_currency_rate_async(currency_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_latest_currency_rate_async: #{e}"
end
```

#### Using the get_latest_currency_rate_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ExchangeRateEnvelope>, Integer, Hash)> get_latest_currency_rate_async_with_http_info(currency_id, opts)

```ruby
begin
  # Get latest rate for a currency
  data, status_code, headers = api_instance.get_latest_currency_rate_async_with_http_info(currency_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ExchangeRateEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_latest_currency_rate_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **currency_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ExchangeRateEnvelope**](ExchangeRateEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_latest_currency_rates_model_async

> <ForexRatesDtoEnvelope> get_latest_currency_rates_model_async(opts)

Get latest currency rates

Retrieves the latest exchange rates for all supported currencies.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::RatesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get latest currency rates
  result = api_instance.get_latest_currency_rates_model_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_latest_currency_rates_model_async: #{e}"
end
```

#### Using the get_latest_currency_rates_model_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ForexRatesDtoEnvelope>, Integer, Hash)> get_latest_currency_rates_model_async_with_http_info(opts)

```ruby
begin
  # Get latest currency rates
  data, status_code, headers = api_instance.get_latest_currency_rates_model_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ForexRatesDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling RatesApi->get_latest_currency_rates_model_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**ForexRatesDtoEnvelope**](ForexRatesDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

