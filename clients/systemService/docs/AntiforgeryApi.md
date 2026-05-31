# OpenapiClient::AntiforgeryApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_and_store_tokens**](AntiforgeryApi.md#get_and_store_tokens) | **GET** /api/v2/SystemService/Antiforgery/GetAndStoreTokens | Get and store antiforgery tokens |
| [**is_request_valid_async**](AntiforgeryApi.md#is_request_valid_async) | **GET** /api/v2/SystemService/Antiforgery/IsRequestValid | Validate antiforgery request |


## get_and_store_tokens

> get_and_store_tokens(opts)

Get and store antiforgery tokens

Generates antiforgery tokens and stores them in the current HTTP context.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AntiforgeryApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get and store antiforgery tokens
  api_instance.get_and_store_tokens(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AntiforgeryApi->get_and_store_tokens: #{e}"
end
```

#### Using the get_and_store_tokens_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_and_store_tokens_with_http_info(opts)

```ruby
begin
  # Get and store antiforgery tokens
  data, status_code, headers = api_instance.get_and_store_tokens_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AntiforgeryApi->get_and_store_tokens_with_http_info: #{e}"
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
- **Accept**: Not defined


## is_request_valid_async

> is_request_valid_async(opts)

Validate antiforgery request

Validates whether the current HTTP request contains a valid antiforgery token.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AntiforgeryApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Validate antiforgery request
  api_instance.is_request_valid_async(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling AntiforgeryApi->is_request_valid_async: #{e}"
end
```

#### Using the is_request_valid_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> is_request_valid_async_with_http_info(opts)

```ruby
begin
  # Validate antiforgery request
  data, status_code, headers = api_instance.is_request_valid_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling AntiforgeryApi->is_request_valid_async_with_http_info: #{e}"
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
- **Accept**: Not defined

