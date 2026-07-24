# OpenapiClient::SignedDocumentAttachmentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#create_signed_document_attachment_async) | **POST** /api/v2/TrustService/SignedDocumentAttachments | Create a new signed document attachment |
| [**delete_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#delete_signed_document_attachment_async) | **DELETE** /api/v2/TrustService/SignedDocumentAttachments/{id} | Delete a signed document attachment |
| [**get_signed_document_attachment_by_id_async**](SignedDocumentAttachmentsApi.md#get_signed_document_attachment_by_id_async) | **GET** /api/v2/TrustService/SignedDocumentAttachments/{id} | Get signed document attachment by ID |
| [**get_signed_document_attachments_async**](SignedDocumentAttachmentsApi.md#get_signed_document_attachments_async) | **GET** /api/v2/TrustService/SignedDocumentAttachments | Get all signed document attachments |
| [**get_signed_document_attachments_count_async**](SignedDocumentAttachmentsApi.md#get_signed_document_attachments_count_async) | **GET** /api/v2/TrustService/SignedDocumentAttachments/Count | Get signed document attachments count |
| [**patch_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#patch_signed_document_attachment_async) | **PATCH** /api/v2/TrustService/SignedDocumentAttachments/{id} | Patch a signed document attachment |
| [**update_signed_document_attachment_async**](SignedDocumentAttachmentsApi.md#update_signed_document_attachment_async) | **PUT** /api/v2/TrustService/SignedDocumentAttachments/{id} | Update a signed document attachment |


## create_signed_document_attachment_async

> create_signed_document_attachment_async(tenant_id, opts)

Create a new signed document attachment

Links an already-stored file to a SignedDocument (metadata + Storage pointer; no bytes).

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signed_document_attachment_create_dto: OpenapiClient::SignedDocumentAttachmentCreateDto.new({signed_document_id: 'signed_document_id_example', title: 'title_example', storage_key: 'storage_key_example'}) # SignedDocumentAttachmentCreateDto | 
}

begin
  # Create a new signed document attachment
  api_instance.create_signed_document_attachment_async(tenant_id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->create_signed_document_attachment_async: #{e}"
end
```

#### Using the create_signed_document_attachment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> create_signed_document_attachment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new signed document attachment
  data, status_code, headers = api_instance.create_signed_document_attachment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->create_signed_document_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signed_document_attachment_create_dto** | [**SignedDocumentAttachmentCreateDto**](SignedDocumentAttachmentCreateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_signed_document_attachment_async

> delete_signed_document_attachment_async(tenant_id, id, opts)

Delete a signed document attachment

Deletes a signed document attachment link for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a signed document attachment
  api_instance.delete_signed_document_attachment_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->delete_signed_document_attachment_async: #{e}"
end
```

#### Using the delete_signed_document_attachment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_signed_document_attachment_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Delete a signed document attachment
  data, status_code, headers = api_instance.delete_signed_document_attachment_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->delete_signed_document_attachment_async_with_http_info: #{e}"
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


## get_signed_document_attachment_by_id_async

> <SignedDocumentAttachmentDto> get_signed_document_attachment_by_id_async(tenant_id, id, opts)

Get signed document attachment by ID

Retrieves a specific signed document attachment by its identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signed document attachment by ID
  result = api_instance.get_signed_document_attachment_by_id_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->get_signed_document_attachment_by_id_async: #{e}"
end
```

#### Using the get_signed_document_attachment_by_id_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignedDocumentAttachmentDto>, Integer, Hash)> get_signed_document_attachment_by_id_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Get signed document attachment by ID
  data, status_code, headers = api_instance.get_signed_document_attachment_by_id_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignedDocumentAttachmentDto>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->get_signed_document_attachment_by_id_async_with_http_info: #{e}"
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

[**SignedDocumentAttachmentDto**](SignedDocumentAttachmentDto.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signed_document_attachments_async

> <SignedDocumentAttachmentDtoListEnvelope> get_signed_document_attachments_async(tenant_id, opts)

Get all signed document attachments

Retrieves all signed document attachments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get all signed document attachments
  result = api_instance.get_signed_document_attachments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->get_signed_document_attachments_async: #{e}"
end
```

#### Using the get_signed_document_attachments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignedDocumentAttachmentDtoListEnvelope>, Integer, Hash)> get_signed_document_attachments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get all signed document attachments
  data, status_code, headers = api_instance.get_signed_document_attachments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignedDocumentAttachmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->get_signed_document_attachments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SignedDocumentAttachmentDtoListEnvelope**](SignedDocumentAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_signed_document_attachments_count_async

> <Int32Envelope> get_signed_document_attachments_count_async(tenant_id, opts)

Get signed document attachments count

Returns the count of signed document attachments for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get signed document attachments count
  result = api_instance.get_signed_document_attachments_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->get_signed_document_attachments_count_async: #{e}"
end
```

#### Using the get_signed_document_attachments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_signed_document_attachments_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get signed document attachments count
  data, status_code, headers = api_instance.get_signed_document_attachments_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->get_signed_document_attachments_count_async_with_http_info: #{e}"
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


## patch_signed_document_attachment_async

> <EmptyEnvelope> patch_signed_document_attachment_async(tenant_id, id, opts)

Patch a signed document attachment

Patch a signed document attachment

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a signed document attachment
  result = api_instance.patch_signed_document_attachment_async(tenant_id, id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->patch_signed_document_attachment_async: #{e}"
end
```

#### Using the patch_signed_document_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_signed_document_attachment_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Patch a signed document attachment
  data, status_code, headers = api_instance.patch_signed_document_attachment_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->patch_signed_document_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **operation** | [**Array&lt;Operation&gt;**](Operation.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## update_signed_document_attachment_async

> update_signed_document_attachment_async(tenant_id, id, opts)

Update a signed document attachment

Updates signed document attachment metadata for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SignedDocumentAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  signed_document_attachment_update_dto: OpenapiClient::SignedDocumentAttachmentUpdateDto.new({title: 'title_example'}) # SignedDocumentAttachmentUpdateDto | 
}

begin
  # Update a signed document attachment
  api_instance.update_signed_document_attachment_async(tenant_id, id, opts)
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->update_signed_document_attachment_async: #{e}"
end
```

#### Using the update_signed_document_attachment_async_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> update_signed_document_attachment_async_with_http_info(tenant_id, id, opts)

```ruby
begin
  # Update a signed document attachment
  data, status_code, headers = api_instance.update_signed_document_attachment_async_with_http_info(tenant_id, id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling SignedDocumentAttachmentsApi->update_signed_document_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **signed_document_attachment_update_dto** | [**SignedDocumentAttachmentUpdateDto**](SignedDocumentAttachmentUpdateDto.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

