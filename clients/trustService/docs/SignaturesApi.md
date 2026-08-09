# OpenapiClient::SignaturesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_signature_by_id_async**](SignaturesApi.md#get_signature_by_id_async) | **GET** /api/v2/TrustService/Signatures/{id} | Get signature by ID |
| [**get_signatures_async**](SignaturesApi.md#get_signatures_async) | **GET** /api/v2/TrustService/Signatures | Get all signatures |
| [**get_signatures_count_async**](SignaturesApi.md#get_signatures_count_async) | **GET** /api/v2/TrustService/Signatures/Count | Get signatures count |


## get_signature_by_id_async

> <SignatureDto> get_signature_by_id_async(tenant_id, id, opts)

Get signature by ID

Retrieves a specific signature by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signature by ID
  result = api_instance.get_signature_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignaturesApi->get_signature_by_id_async: #{e}"
end
```

#### Using the get_signature_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignatureDto>, Integer, Hash)> get_signature_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signature by ID
  data, status_code, headers = api_instance.get_signature_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignatureDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignaturesApi->get_signature_by_id_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SignatureDto**](SignatureDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signatures_async

> <SignatureDtoListEnvelope> get_signatures_async(tenant_id, opts)

Get all signatures

Retrieves all signatures for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signature_dto_collection_query_parameters: OpenapiClient::SignatureDtoCollectionQueryParameters.new # SignatureDtoCollectionQueryParameters | 
}

begin
  # Get all signatures
  result = api_instance.get_signatures_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignaturesApi->get_signatures_async: #{e}"
end
```

#### Using the get_signatures_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignatureDtoListEnvelope>, Integer, Hash)> get_signatures_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signatures
  data, status_code, headers = api_instance.get_signatures_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignatureDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignaturesApi->get_signatures_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signature_dto_collection_query_parameters** | [**SignatureDtoCollectionQueryParameters**](SignatureDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SignatureDtoListEnvelope**](SignatureDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signatures_count_async

> <Int32Envelope> get_signatures_count_async(tenant_id, opts)

Get signatures count

Returns the count of signatures for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignaturesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signature_dto_collection_query_parameters: OpenapiClient::SignatureDtoCollectionQueryParameters.new # SignatureDtoCollectionQueryParameters | 
}

begin
  # Get signatures count
  result = api_instance.get_signatures_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignaturesApi->get_signatures_count_async: #{e}"
end
```

#### Using the get_signatures_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signatures_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signatures count
  data, status_code, headers = api_instance.get_signatures_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignaturesApi->get_signatures_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signature_dto_collection_query_parameters** | [**SignatureDtoCollectionQueryParameters**](SignatureDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

