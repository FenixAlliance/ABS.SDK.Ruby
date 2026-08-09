# OpenapiClient::SignedDocumentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_signed_document_async**](SignedDocumentsApi.md#create_signed_document_async) | **POST** /api/v2/TrustService/SignedDocuments | Create a new signed document |
| [**delete_signed_document_async**](SignedDocumentsApi.md#delete_signed_document_async) | **DELETE** /api/v2/TrustService/SignedDocuments/{id} | Delete a signed document |
| [**get_signed_document_by_id_async**](SignedDocumentsApi.md#get_signed_document_by_id_async) | **GET** /api/v2/TrustService/SignedDocuments/{id} | Get signed document by ID |
| [**get_signed_documents_async**](SignedDocumentsApi.md#get_signed_documents_async) | **GET** /api/v2/TrustService/SignedDocuments | Get all signed documents |
| [**get_signed_documents_count_async**](SignedDocumentsApi.md#get_signed_documents_count_async) | **GET** /api/v2/TrustService/SignedDocuments/Count | Get signed documents count |
| [**patch_signed_document_async**](SignedDocumentsApi.md#patch_signed_document_async) | **PATCH** /api/v2/TrustService/SignedDocuments/{id} | Patch a signed document |
| [**prepare_and_quick_sign_async**](SignedDocumentsApi.md#prepare_and_quick_sign_async) | **POST** /api/v2/TrustService/SignedDocuments/prepare-and-quick-sign | Create, freeze, and quick-sign a document in one call |
| [**quick_sign_signed_document_async**](SignedDocumentsApi.md#quick_sign_signed_document_async) | **POST** /api/v2/TrustService/SignedDocuments/{id}/quick-sign | Quick-sign a frozen document |
| [**update_signed_document_async**](SignedDocumentsApi.md#update_signed_document_async) | **PUT** /api/v2/TrustService/SignedDocuments/{id} | Update a signed document |
| [**verify_signed_document_signature_async**](SignedDocumentsApi.md#verify_signed_document_signature_async) | **GET** /api/v2/TrustService/SignedDocuments/{id}/verify-signature | Verify a signed document&#39;s signature |


## create_signed_document_async

> create_signed_document_async(tenant_id, opts)

Create a new signed document

Creates a new signed document for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signed_document_create_dto: OpenapiClient::SignedDocumentCreateDto.new({title: 'title_example', contact_id: 'contact_id_example'}) # SignedDocumentCreateDto | 
}

begin
  # Create a new signed document
  api_instance.create_signed_document_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->create_signed_document_async: #{e}"
end
```

#### Using the create_signed_document_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_signed_document_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new signed document
  data, status_code, headers = api_instance.create_signed_document_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->create_signed_document_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signed_document_create_dto** | [**SignedDocumentCreateDto**](SignedDocumentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_signed_document_async

> delete_signed_document_async(tenant_id, id, opts)

Delete a signed document

Deletes a signed document for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a signed document
  api_instance.delete_signed_document_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->delete_signed_document_async: #{e}"
end
```

#### Using the delete_signed_document_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_signed_document_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a signed document
  data, status_code, headers = api_instance.delete_signed_document_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->delete_signed_document_async_with_http_info: #{e}"
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

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signed_document_by_id_async

> <SignedDocumentDto> get_signed_document_by_id_async(tenant_id, id, opts)

Get signed document by ID

Retrieves a specific signed document by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signed document by ID
  result = api_instance.get_signed_document_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->get_signed_document_by_id_async: #{e}"
end
```

#### Using the get_signed_document_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignedDocumentDto>, Integer, Hash)> get_signed_document_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signed document by ID
  data, status_code, headers = api_instance.get_signed_document_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignedDocumentDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->get_signed_document_by_id_async_with_http_info: #{e}"
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

[**SignedDocumentDto**](SignedDocumentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signed_documents_async

> <SignedDocumentDtoListEnvelope> get_signed_documents_async(tenant_id, opts)

Get all signed documents

Retrieves all signed documents for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signed_document_dto_collection_query_parameters: OpenapiClient::SignedDocumentDtoCollectionQueryParameters.new # SignedDocumentDtoCollectionQueryParameters | 
}

begin
  # Get all signed documents
  result = api_instance.get_signed_documents_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->get_signed_documents_async: #{e}"
end
```

#### Using the get_signed_documents_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignedDocumentDtoListEnvelope>, Integer, Hash)> get_signed_documents_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signed documents
  data, status_code, headers = api_instance.get_signed_documents_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignedDocumentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->get_signed_documents_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signed_document_dto_collection_query_parameters** | [**SignedDocumentDtoCollectionQueryParameters**](SignedDocumentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**SignedDocumentDtoListEnvelope**](SignedDocumentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## get_signed_documents_count_async

> <Int32Envelope> get_signed_documents_count_async(tenant_id, opts)

Get signed documents count

Returns the count of signed documents for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signed_document_dto_collection_query_parameters: OpenapiClient::SignedDocumentDtoCollectionQueryParameters.new # SignedDocumentDtoCollectionQueryParameters | 
}

begin
  # Get signed documents count
  result = api_instance.get_signed_documents_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->get_signed_documents_count_async: #{e}"
end
```

#### Using the get_signed_documents_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signed_documents_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signed documents count
  data, status_code, headers = api_instance.get_signed_documents_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->get_signed_documents_count_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signed_document_dto_collection_query_parameters** | [**SignedDocumentDtoCollectionQueryParameters**](SignedDocumentDtoCollectionQueryParameters.md) |  | [optional] |

### Return type

[**Int32Envelope**](Int32Envelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## patch_signed_document_async

> <EmptyEnvelope> patch_signed_document_async(tenant_id, id, opts)

Patch a signed document

Patch a signed document

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  patch_operation: [OpenapiClient::PatchOperation.new] # Array<PatchOperation> | 
}

begin
  # Patch a signed document
  result = api_instance.patch_signed_document_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->patch_signed_document_async: #{e}"
end
```

#### Using the patch_signed_document_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_signed_document_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a signed document
  data, status_code, headers = api_instance.patch_signed_document_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->patch_signed_document_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **patch_operation** | [**Array&lt;PatchOperation&gt;**](PatchOperation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## prepare_and_quick_sign_async

> <SignedDocumentDto> prepare_and_quick_sign_async(tenant_id, opts)

Create, freeze, and quick-sign a document in one call

Server-side single-signer flow: creates a SignedDocument from the uploaded source, stores it, freezes it, signs it with the chosen certificate + provider, and seals it — all in one unit of work. Returns the sealed document. Evidence truth (signed/status/hashes/artifact ids) is server-produced and cannot be supplied by the caller.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  id: '38400000-8cf0-11bd-b23e-10b96e4ef00d', # String | 
  file: File.new('/path/to/some/file'), # File | 
  title: 'title_example', # String | 
  contact_id: 'contact_id_example', # String | 
  signing_certificate_id: 'signing_certificate_id_example', # String | 
  signing_profile_id: 'signing_profile_id_example', # String | 
  provider_name: 'provider_name_example' # String | 
}

begin
  # Create, freeze, and quick-sign a document in one call
  result = api_instance.prepare_and_quick_sign_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->prepare_and_quick_sign_async: #{e}"
end
```

#### Using the prepare_and_quick_sign_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignedDocumentDto>, Integer, Hash)> prepare_and_quick_sign_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create, freeze, and quick-sign a document in one call
  data, status_code, headers = api_instance.prepare_and_quick_sign_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignedDocumentDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->prepare_and_quick_sign_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **id** | **String** |  | [optional] |
| **file** | **File** |  | [optional] |
| **title** | **String** |  | [optional] |
| **contact_id** | **String** |  | [optional] |
| **signing_certificate_id** | **String** |  | [optional] |
| **signing_profile_id** | **String** |  | [optional] |
| **provider_name** | **String** |  | [optional] |

### Return type

[**SignedDocumentDto**](SignedDocumentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json, application/xml
- **Accept**: application/json, application/xml


## quick_sign_signed_document_async

> quick_sign_signed_document_async(tenant_id, id, opts)

Quick-sign a frozen document

Signs a frozen signed document directly with a chosen certificate + provider (no signing-request workflow) and seals it. Returns the sealed document.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  quick_sign_signed_document_dto: OpenapiClient::QuickSignSignedDocumentDto.new({provider_name: 'provider_name_example', signing_certificate_id: 'signing_certificate_id_example'}) # QuickSignSignedDocumentDto | 
}

begin
  # Quick-sign a frozen document
  api_instance.quick_sign_signed_document_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->quick_sign_signed_document_async: #{e}"
end
```

#### Using the quick_sign_signed_document_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> quick_sign_signed_document_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Quick-sign a frozen document
  data, status_code, headers = api_instance.quick_sign_signed_document_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->quick_sign_signed_document_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **quick_sign_signed_document_dto** | [**QuickSignSignedDocumentDto**](QuickSignSignedDocumentDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_signed_document_async

> update_signed_document_async(tenant_id, id, opts)

Update a signed document

Updates an existing signed document for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signed_document_update_dto: OpenapiClient::SignedDocumentUpdateDto.new({title: 'title_example', contact_id: 'contact_id_example'}) # SignedDocumentUpdateDto | 
}

begin
  # Update a signed document
  api_instance.update_signed_document_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->update_signed_document_async: #{e}"
end
```

#### Using the update_signed_document_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_signed_document_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a signed document
  data, status_code, headers = api_instance.update_signed_document_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->update_signed_document_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signed_document_update_dto** | [**SignedDocumentUpdateDto**](SignedDocumentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## verify_signed_document_signature_async

> <SignatureVerificationDto> verify_signed_document_signature_async(tenant_id, id, opts)

Verify a signed document's signature

Re-verifies the document's signature against its stored signed artifact (bytes intact + signed by the embedded certificate; certificate trust is a separate concern).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Verify a signed document's signature
  result = api_instance.verify_signed_document_signature_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->verify_signed_document_signature_async: #{e}"
end
```

#### Using the verify_signed_document_signature_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignatureVerificationDto>, Integer, Hash)> verify_signed_document_signature_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Verify a signed document's signature
  data, status_code, headers = api_instance.verify_signed_document_signature_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignatureVerificationDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentsApi->verify_signed_document_signature_async_with_http_info: #{e}"
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

[**SignatureVerificationDto**](SignatureVerificationDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

