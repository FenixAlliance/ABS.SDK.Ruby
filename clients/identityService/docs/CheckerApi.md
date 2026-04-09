# OpenapiClient::CheckerApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**is_authenticated**](CheckerApi.md#is_authenticated) | **GET** /api/v2/Auth/Checker/IsAuthenticated | Check if user is authenticated |


## is_authenticated

> Boolean is_authenticated(opts)

Check if user is authenticated

Returns whether the current user is authenticated.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CheckerApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Check if user is authenticated
  result = api_instance.is_authenticated(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CheckerApi->is_authenticated: #{e}"
end
```

#### Using the is_authenticated_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Boolean, Integer, Hash)> is_authenticated_with_http_info(opts)

```ruby
begin
  # Check if user is authenticated
  data, status_code, headers = api_instance.is_authenticated_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Boolean
rescue OpenapiClient::ApiError => e
  puts "Error when calling CheckerApi->is_authenticated_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

**Boolean**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

