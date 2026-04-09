# OpenapiClient::ResourceApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_message**](ResourceApi.md#get_message) | **GET** /api/v2/IdentityService/Resource/message | Get authenticated resource message |


## get_message

> get_message(opts)

Get authenticated resource message

Returns a message confirming the authenticated user's identity. Requires the 'abs_api' scope.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::ResourceApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get authenticated resource message
  api_instance.get_message(opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling ResourceApi->get_message: #{e}"
end
```

#### Using the get_message_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> get_message_with_http_info(opts)

```ruby
begin
  # Get authenticated resource message
  data, status_code, headers = api_instance.get_message_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling ResourceApi->get_message_with_http_info: #{e}"
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

