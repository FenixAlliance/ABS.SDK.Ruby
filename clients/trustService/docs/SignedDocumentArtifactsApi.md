# OpenapiClient::SignedDocumentArtifactsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**freeze_async**](SignedDocumentArtifactsApi.md#freeze_async) | **POST** /api/v2/TrustService/SignedDocumentArtifacts/{signedDocumentId}/freeze | Freeze the source for signature |
| [**get_reference_async**](SignedDocumentArtifactsApi.md#get_reference_async) | **GET** /api/v2/TrustService/SignedDocumentArtifacts/reference/{fileUploadId} | Get an artifact reference |
| [**set_primary_authoring_file_async**](SignedDocumentArtifactsApi.md#set_primary_authoring_file_async) | **PUT** /api/v2/TrustService/SignedDocumentArtifacts/{signedDocumentId}/primary-file/{fileUploadId} | Set the primary authoring file |
| [**verify_async**](SignedDocumentArtifactsApi.md#verify_async) | **GET** /api/v2/TrustService/SignedDocumentArtifacts/reference/{fileUploadId}/verify | Verify an artifact hash |


## freeze_async

> <TrustArtifactReferenceDtoEnvelope> freeze_async(tenant_id, signed_document_id, opts)

Freeze the source for signature

Copies the primary authoring artifact into a new Sealed frozen-source artifact, hashes it, and binds it to the document (LockState = FrozenForSignature).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentArtifactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
signed_document_id = 'signed_document_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Freeze the source for signature
  result = api_instance.freeze_async(tenant_id, signed_document_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->freeze_async: #{e}"
end
```

#### Using the freeze_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrustArtifactReferenceDtoEnvelope>, Integer, Hash)> freeze_async_with_http_info(tenant_id, signed_document_id, opts)

```ruby
begin
  # Freeze the source for signature
  data, status_code, headers = api_instance.freeze_async_with_http_info(tenant_id, signed_document_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrustArtifactReferenceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->freeze_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **signed_document_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrustArtifactReferenceDtoEnvelope**](TrustArtifactReferenceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_reference_async

> <TrustArtifactReferenceDtoEnvelope> get_reference_async(tenant_id, file_upload_id, opts)

Get an artifact reference

Resolves a stored artifact's reference (FileUpload id + key + hash + media hints).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentArtifactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
file_upload_id = 'file_upload_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get an artifact reference
  result = api_instance.get_reference_async(tenant_id, file_upload_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->get_reference_async: #{e}"
end
```

#### Using the get_reference_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TrustArtifactReferenceDtoEnvelope>, Integer, Hash)> get_reference_async_with_http_info(tenant_id, file_upload_id, opts)

```ruby
begin
  # Get an artifact reference
  data, status_code, headers = api_instance.get_reference_async_with_http_info(tenant_id, file_upload_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TrustArtifactReferenceDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->get_reference_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **file_upload_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**TrustArtifactReferenceDtoEnvelope**](TrustArtifactReferenceDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## set_primary_authoring_file_async

> set_primary_authoring_file_async(tenant_id, signed_document_id, file_upload_id, opts)

Set the primary authoring file

Links an existing scan-gated FileUpload as the document's mutable authoring artifact (only while editable).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentArtifactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
signed_document_id = 'signed_document_id_example' # String | 
file_upload_id = 'file_upload_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Set the primary authoring file
  api_instance.set_primary_authoring_file_async(tenant_id, signed_document_id, file_upload_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->set_primary_authoring_file_async: #{e}"
end
```

#### Using the set_primary_authoring_file_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> set_primary_authoring_file_async_with_http_info(tenant_id, signed_document_id, file_upload_id, opts)

```ruby
begin
  # Set the primary authoring file
  data, status_code, headers = api_instance.set_primary_authoring_file_async_with_http_info(tenant_id, signed_document_id, file_upload_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->set_primary_authoring_file_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **signed_document_id** | **String** |  |  |
| **file_upload_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## verify_async

> <BooleanEnvelope> verify_async(tenant_id, file_upload_id, opts)

Verify an artifact hash

Re-reads the artifact bytes and verifies them against the recorded SHA-256. Returns true on match.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentArtifactsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
file_upload_id = 'file_upload_id_example' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Verify an artifact hash
  result = api_instance.verify_async(tenant_id, file_upload_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->verify_async: #{e}"
end
```

#### Using the verify_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BooleanEnvelope>, Integer, Hash)> verify_async_with_http_info(tenant_id, file_upload_id, opts)

```ruby
begin
  # Verify an artifact hash
  data, status_code, headers = api_instance.verify_async_with_http_info(tenant_id, file_upload_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BooleanEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentArtifactsApi->verify_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **file_upload_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**BooleanEnvelope**](BooleanEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

