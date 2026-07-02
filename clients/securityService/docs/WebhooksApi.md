# OpenapiClient::WebhooksApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_webhook_requests_async**](WebhooksApi.md#get_webhook_requests_async) | **GET** /api/v2/SecurityService/Webhooks | Get all webhook requests |
| [**get_webhook_requests_count_async**](WebhooksApi.md#get_webhook_requests_count_async) | **GET** /api/v2/SecurityService/Webhooks/Count | Get webhook requests count |


## get_webhook_requests_async

> <WebhookRequestDtoListEnvelope> get_webhook_requests_async(tenant_id, opts)

Get all webhook requests

Retrieves all webhook requests for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebhooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all webhook requests
  result = api_instance.get_webhook_requests_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->get_webhook_requests_async: #{e}"
end
```

#### Using the get_webhook_requests_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebhookRequestDtoListEnvelope>, Integer, Hash)> get_webhook_requests_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all webhook requests
  data, status_code, headers = api_instance.get_webhook_requests_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebhookRequestDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->get_webhook_requests_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**WebhookRequestDtoListEnvelope**](WebhookRequestDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_webhook_requests_count_async

> <Int32Envelope> get_webhook_requests_count_async(tenant_id, opts)

Get webhook requests count

Retrieves the count of webhook requests for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebhooksApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get webhook requests count
  result = api_instance.get_webhook_requests_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->get_webhook_requests_count_async: #{e}"
end
```

#### Using the get_webhook_requests_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_webhook_requests_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get webhook requests count
  data, status_code, headers = api_instance.get_webhook_requests_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->get_webhook_requests_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

