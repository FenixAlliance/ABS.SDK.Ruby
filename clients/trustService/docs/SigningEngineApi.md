# OpenapiClient::SigningEngineApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_providers_async**](SigningEngineApi.md#get_providers_async) | **GET** /api/v2/TrustService/SigningEngine/Providers | List signing providers |
| [**get_providers_count_async**](SigningEngineApi.md#get_providers_count_async) | **GET** /api/v2/TrustService/SigningEngine/Providers/Count | Count signing providers |
| [**preview_async**](SigningEngineApi.md#preview_async) | **POST** /api/v2/TrustService/SigningEngine/Preview | Preview signing readiness |


## get_providers_async

> <TrustSigningProviderDescriptorDtoListEnvelope> get_providers_async(tenant_id, opts)

List signing providers

Returns the registered alpha signing providers (Noop / Manual / External). OData-queryable.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningEngineApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # List signing providers
  result = api_instance.get_providers_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningEngineApi->get_providers_async: #{e}"
end
```

#### Using the get_providers_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrustSigningProviderDescriptorDtoListEnvelope>, Integer, Hash)> get_providers_async_with_http_info(tenant_id, opts)

```ruby
begin
  # List signing providers
  data, status_code, headers = api_instance.get_providers_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrustSigningProviderDescriptorDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningEngineApi->get_providers_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrustSigningProviderDescriptorDtoListEnvelope**](TrustSigningProviderDescriptorDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_providers_count_async

> <Int32Envelope> get_providers_count_async(tenant_id, opts)

Count signing providers

Returns the count of registered alpha signing providers. OData-queryable.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningEngineApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Count signing providers
  result = api_instance.get_providers_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningEngineApi->get_providers_count_async: #{e}"
end
```

#### Using the get_providers_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_providers_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Count signing providers
  data, status_code, headers = api_instance.get_providers_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningEngineApi->get_providers_count_async_with_http_info: #{e}"
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


## preview_async

> <TrustSigningReadinessDtoEnvelope> preview_async(tenant_id, opts)

Preview signing readiness

Side-effect-free: validates a signing request and reports whether it can proceed and with what policy.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SigningEngineApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  trust_signing_request_dto: OpenapiClient::TrustSigningRequestDto.new # TrustSigningRequestDto | 
}

begin
  # Preview signing readiness
  result = api_instance.preview_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningEngineApi->preview_async: #{e}"
end
```

#### Using the preview_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrustSigningReadinessDtoEnvelope>, Integer, Hash)> preview_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Preview signing readiness
  data, status_code, headers = api_instance.preview_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrustSigningReadinessDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SigningEngineApi->preview_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **trust_signing_request_dto** | [**TrustSigningRequestDto**](TrustSigningRequestDto.md) |  | [optional] |

### Return type

[**TrustSigningReadinessDtoEnvelope**](TrustSigningReadinessDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

