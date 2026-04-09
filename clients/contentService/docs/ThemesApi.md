# OpenapiClient::ThemesApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_latest_currency_rates_model_async**](ThemesApi.md#get_latest_currency_rates_model_async) | **GET** /api/v2/ContentService/Themes/Update | Update base web content themes |


## get_latest_currency_rates_model_async

> get_latest_currency_rates_model_async(opts)

Update base web content themes

Triggers an update of the base web content themes.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ThemesApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Update base web content themes
  api_instance.get_latest_currency_rates_model_async(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ThemesApi->get_latest_currency_rates_model_async: #{e}"
end
```

#### Using the get_latest_currency_rates_model_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_latest_currency_rates_model_async_with_http_info(opts)

```ruby
begin
  # Update base web content themes
  data, status_code, headers = api_instance.get_latest_currency_rates_model_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ThemesApi->get_latest_currency_rates_model_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

