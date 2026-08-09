# OpenapiClient::SecurityCertificatesApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_security_certificates_async**](SecurityCertificatesApi.md#get_security_certificates_async) | **GET** /api/v2/SecurityService/SecurityCertificates | Get security certificates |
| [**get_security_certificates_count_async**](SecurityCertificatesApi.md#get_security_certificates_count_async) | **GET** /api/v2/SecurityService/SecurityCertificates/Count | Get security certificates count |


## get_security_certificates_async

> <SecurityCertificateDtoListEnvelope> get_security_certificates_async(tenant_id, opts)

Get security certificates

Retrieves security certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SecurityCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  security_certificate_dto_collection_query_parameters: OpenapiClient::SecurityCertificateDtoCollectionQueryParameters.new # SecurityCertificateDtoCollectionQueryParameters | 
}

begin
  # Get security certificates
  result = api_instance.get_security_certificates_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityCertificatesApi->get_security_certificates_async: #{e}"
end
```

#### Using the get_security_certificates_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SecurityCertificateDtoListEnvelope>, Integer, Hash)> get_security_certificates_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get security certificates
  data, status_code, headers = api_instance.get_security_certificates_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SecurityCertificateDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityCertificatesApi->get_security_certificates_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **security_certificate_dto_collection_query_parameters** | [**SecurityCertificateDtoCollectionQueryParameters**](SecurityCertificateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SecurityCertificateDtoListEnvelope**](SecurityCertificateDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_security_certificates_count_async

> <Int32Envelope> get_security_certificates_count_async(tenant_id, opts)

Get security certificates count

Retrieves the count of security certificates for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SecurityCertificatesApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  security_certificate_dto_collection_query_parameters: OpenapiClient::SecurityCertificateDtoCollectionQueryParameters.new # SecurityCertificateDtoCollectionQueryParameters | 
}

begin
  # Get security certificates count
  result = api_instance.get_security_certificates_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityCertificatesApi->get_security_certificates_count_async: #{e}"
end
```

#### Using the get_security_certificates_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_security_certificates_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get security certificates count
  data, status_code, headers = api_instance.get_security_certificates_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SecurityCertificatesApi->get_security_certificates_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **security_certificate_dto_collection_query_parameters** | [**SecurityCertificateDtoCollectionQueryParameters**](SecurityCertificateDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

