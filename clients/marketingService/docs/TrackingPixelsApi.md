# OpenapiClient::TrackingPixelsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_tracking_pixel_async**](TrackingPixelsApi.md#get_tracking_pixel_async) | **GET** /api/v2/MarketingService/TrackingPixels/{pixelId} | Get a tracking pixel |


## get_tracking_pixel_async

> <OrderDtoEnvelope> get_tracking_pixel_async(pixel_id, opts)

Get a tracking pixel

Retrieves a tracking pixel by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::TrackingPixelsApi.new
pixel_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a tracking pixel
  result = api_instance.get_tracking_pixel_async(pixel_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrackingPixelsApi->get_tracking_pixel_async: #{e}"
end
```

#### Using the get_tracking_pixel_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<OrderDtoEnvelope>, Integer, Hash)> get_tracking_pixel_async_with_http_info(pixel_id, opts)

```ruby
begin
  # Get a tracking pixel
  data, status_code, headers = api_instance.get_tracking_pixel_async_with_http_info(pixel_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <OrderDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TrackingPixelsApi->get_tracking_pixel_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **pixel_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**OrderDtoEnvelope**](OrderDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

