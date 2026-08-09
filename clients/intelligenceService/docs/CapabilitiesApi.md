# OpenapiClient::CapabilitiesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_capabilities_async**](CapabilitiesApi.md#get_capabilities_async) | **GET** /api/v2/IntelligenceService/Capabilities | Get the annotated capability catalog |
| [**get_capabilities_count_async**](CapabilitiesApi.md#get_capabilities_count_async) | **GET** /api/v2/IntelligenceService/Capabilities/Count | Get the capability catalog count |
| [**get_capability_by_key_async**](CapabilitiesApi.md#get_capability_by_key_async) | **GET** /api/v2/IntelligenceService/Capabilities/{key} | Get a capability by key |


## get_capabilities_async

> <CapabilityDtoListEnvelope> get_capabilities_async(tenant_id, opts)

Get the annotated capability catalog

Retrieves the full governed-capability catalog for the specified tenant, optionally narrowed to a single execution surface. Every capability is returned with an Available flag (and a DeniedReason when not available) so callers render disabled-with-reason instead of hiding; entitlement is computed server-side.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CapabilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  surface: 'None', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the annotated capability catalog
  result = api_instance.get_capabilities_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CapabilitiesApi->get_capabilities_async: #{e}"
end
```

#### Using the get_capabilities_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CapabilityDtoListEnvelope>, Integer, Hash)> get_capabilities_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the annotated capability catalog
  data, status_code, headers = api_instance.get_capabilities_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CapabilityDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CapabilitiesApi->get_capabilities_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **surface** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CapabilityDtoListEnvelope**](CapabilityDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_capabilities_count_async

> <Int32Envelope> get_capabilities_count_async(tenant_id, opts)

Get the capability catalog count

Returns the number of governed capabilities in the catalog for the specified tenant — the surface-matching total that mirrors the list route's returned-set size (entitled or not), honouring the same optional surface narrowing.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CapabilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  surface: 'None', # String | 
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the capability catalog count
  result = api_instance.get_capabilities_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CapabilitiesApi->get_capabilities_count_async: #{e}"
end
```

#### Using the get_capabilities_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_capabilities_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the capability catalog count
  data, status_code, headers = api_instance.get_capabilities_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CapabilitiesApi->get_capabilities_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **surface** | **String** |  | [optional] |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_capability_by_key_async

> <CapabilityDtoEnvelope> get_capability_by_key_async(tenant_id, key, opts)

Get a capability by key

Retrieves a single governed capability by its stable, dotted key, stamped with the Available / DeniedReason entitlement flag. Returns 404 only when the capability does not exist; an existing capability the actor is not entitled to run is returned annotated as unavailable, not hidden.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::CapabilitiesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
key = 'key_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get a capability by key
  result = api_instance.get_capability_by_key_async(tenant_id, key, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CapabilitiesApi->get_capability_by_key_async: #{e}"
end
```

#### Using the get_capability_by_key_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CapabilityDtoEnvelope>, Integer, Hash)> get_capability_by_key_async_with_http_info(tenant_id, key, opts)

```ruby
begin
  # Get a capability by key
  data, status_code, headers = api_instance.get_capability_by_key_async_with_http_info(tenant_id, key, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CapabilityDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CapabilitiesApi->get_capability_by_key_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **key** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**CapabilityDtoEnvelope**](CapabilityDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

