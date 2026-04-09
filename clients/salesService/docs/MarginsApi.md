# OpenapiClient::MarginsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_quote_async**](MarginsApi.md#get_quote_async) | **GET** /api/v2/SalesService/Margins/{marginId}/Details | Get margin details by ID |


## get_quote_async

> get_quote_async(margin_id, opts)

Get margin details by ID

Retrieves the details of a specific sales margin by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::MarginsApi.new
margin_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get margin details by ID
  api_instance.get_quote_async(margin_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarginsApi->get_quote_async: #{e}"
end
```

#### Using the get_quote_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_quote_async_with_http_info(margin_id, opts)

```ruby
begin
  # Get margin details by ID
  data, status_code, headers = api_instance.get_quote_async_with_http_info(margin_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling MarginsApi->get_quote_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **margin_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

