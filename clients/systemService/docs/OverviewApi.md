# OpenapiClient::OverviewApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_system_overview**](OverviewApi.md#get_system_overview) | **GET** /api/v2/SystemService/Overview | Get system overview information |


## get_system_overview

> <SystemOverviewDtoEnvelope> get_system_overview(opts)

Get system overview information

Returns runtime, memory, and entity count information for the system

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::OverviewApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get system overview information
  result = api_instance.get_system_overview(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling OverviewApi->get_system_overview: #{e}"
end
```

#### Using the get_system_overview_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SystemOverviewDtoEnvelope>, Integer, Hash)> get_system_overview_with_http_info(opts)

```ruby
begin
  # Get system overview information
  data, status_code, headers = api_instance.get_system_overview_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SystemOverviewDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling OverviewApi->get_system_overview_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SystemOverviewDtoEnvelope**](SystemOverviewDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

