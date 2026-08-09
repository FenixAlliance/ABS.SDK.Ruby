# OpenapiClient::AiProvidersApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_ai_providers_async**](AiProvidersApi.md#get_ai_providers_async) | **GET** /api/v2/IntelligenceService/AiProviders | Get the available AI providers |


## get_ai_providers_async

> <AiProviderDtoListEnvelope> get_ai_providers_async(opts)

Get the available AI providers

Returns every AI provider key this instance has a registered adapter for. The set is a property of the deployment, so it is not tenant-scoped; what varies per tenant is the credential for a provider, which is never returned here.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::AiProvidersApi.new
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the available AI providers
  result = api_instance.get_ai_providers_async(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling AiProvidersApi->get_ai_providers_async: #{e}"
end
```

#### Using the get_ai_providers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AiProviderDtoListEnvelope>, Integer, Hash)> get_ai_providers_async_with_http_info(opts)

```ruby
begin
  # Get the available AI providers
  data, status_code, headers = api_instance.get_ai_providers_async_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AiProviderDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling AiProvidersApi->get_ai_providers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**AiProviderDtoListEnvelope**](AiProviderDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

