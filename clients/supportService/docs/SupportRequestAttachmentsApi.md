# OpenapiClient::SupportRequestAttachmentsApi

All URIs are relative to *https://absuite.net*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_support_request_attachment_async**](SupportRequestAttachmentsApi.md#create_support_request_attachment_async) | **POST** /api/v2/SupportService/SupportRequestAttachments | Create a new support request attachment |
| [**delete_support_request_attachment_async**](SupportRequestAttachmentsApi.md#delete_support_request_attachment_async) | **DELETE** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Delete a support request attachment |
| [**get_support_request_attachment_async**](SupportRequestAttachmentsApi.md#get_support_request_attachment_async) | **GET** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Retrieve a support request attachment by ID |
| [**get_support_request_attachments_async**](SupportRequestAttachmentsApi.md#get_support_request_attachments_async) | **GET** /api/v2/SupportService/SupportRequestAttachments | Retrieve a list of support request attachments |
| [**get_support_request_attachments_count_async**](SupportRequestAttachmentsApi.md#get_support_request_attachments_count_async) | **GET** /api/v2/SupportService/SupportRequestAttachments/Count | Get the count of support request attachments |
| [**patch_support_request_attachment_async**](SupportRequestAttachmentsApi.md#patch_support_request_attachment_async) | **PATCH** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Patch a support request attachment |
| [**update_support_request_attachment_async**](SupportRequestAttachmentsApi.md#update_support_request_attachment_async) | **PUT** /api/v2/SupportService/SupportRequestAttachments/{supportRequestAttachmentId} | Update a support request attachment |


## create_support_request_attachment_async

> <EmptyEnvelope> create_support_request_attachment_async(tenant_id, opts)

Create a new support request attachment

Creates a new support request attachment for the specified tenant.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_request_attachment_create_dto: OpenapiClient::SupportRequestAttachmentCreateDto.new # SupportRequestAttachmentCreateDto | 
}

begin
  # Create a new support request attachment
  result = api_instance.create_support_request_attachment_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->create_support_request_attachment_async: #{e}"
end
```

#### Using the create_support_request_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> create_support_request_attachment_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Create a new support request attachment
  data, status_code, headers = api_instance.create_support_request_attachment_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->create_support_request_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_request_attachment_create_dto** | [**SupportRequestAttachmentCreateDto**](SupportRequestAttachmentCreateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml


## delete_support_request_attachment_async

> <EmptyEnvelope> delete_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)

Delete a support request attachment

Deletes a support request attachment by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Delete a support request attachment
  result = api_instance.delete_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->delete_support_request_attachment_async: #{e}"
end
```

#### Using the delete_support_request_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> delete_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)

```ruby
begin
  # Delete a support request attachment
  data, status_code, headers = api_instance.delete_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->delete_support_request_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_attachment_async

> <SupportRequestAttachmentDtoEnvelope> get_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)

Retrieve a support request attachment by ID

Retrieves a single support request attachment by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a support request attachment by ID
  result = api_instance.get_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->get_support_request_attachment_async: #{e}"
end
```

#### Using the get_support_request_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportRequestAttachmentDtoEnvelope>, Integer, Hash)> get_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)

```ruby
begin
  # Retrieve a support request attachment by ID
  data, status_code, headers = api_instance.get_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportRequestAttachmentDtoEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->get_support_request_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportRequestAttachmentDtoEnvelope**](SupportRequestAttachmentDtoEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_attachments_async

> <SupportRequestAttachmentDtoListEnvelope> get_support_request_attachments_async(tenant_id, opts)

Retrieve a list of support request attachments

Retrieves a list of support request attachments for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Retrieve a list of support request attachments
  result = api_instance.get_support_request_attachments_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->get_support_request_attachments_async: #{e}"
end
```

#### Using the get_support_request_attachments_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SupportRequestAttachmentDtoListEnvelope>, Integer, Hash)> get_support_request_attachments_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Retrieve a list of support request attachments
  data, status_code, headers = api_instance.get_support_request_attachments_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SupportRequestAttachmentDtoListEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->get_support_request_attachments_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |

### Return type

[**SupportRequestAttachmentDtoListEnvelope**](SupportRequestAttachmentDtoListEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml


## get_support_request_attachments_count_async

> <Int32Envelope> get_support_request_attachments_count_async(tenant_id, opts)

Get the count of support request attachments

Returns the total count of support request attachments for the specified tenant with OData query support.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example' # String | 
}

begin
  # Get the count of support request attachments
  result = api_instance.get_support_request_attachments_count_async(tenant_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->get_support_request_attachments_count_async: #{e}"
end
```

#### Using the get_support_request_attachments_count_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Int32Envelope>, Integer, Hash)> get_support_request_attachments_count_async_with_http_info(tenant_id, opts)

```ruby
begin
  # Get the count of support request attachments
  data, status_code, headers = api_instance.get_support_request_attachments_count_async_with_http_info(tenant_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Int32Envelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->get_support_request_attachments_count_async_with_http_info: #{e}"
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


## patch_support_request_attachment_async

> <EmptyEnvelope> patch_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)

Patch a support request attachment

Partially updates an existing support request attachment by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  operation: [OpenapiClient::Operation.new] # Array<Operation> | 
}

begin
  # Patch a support request attachment
  result = api_instance.patch_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->patch_support_request_attachment_async: #{e}"
end
```

#### Using the patch_support_request_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> patch_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)

```ruby
begin
  # Patch a support request attachment
  data, status_code, headers = api_instance.patch_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->patch_support_request_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_attachment_id** | **String** |  |  |
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


## update_support_request_attachment_async

> <EmptyEnvelope> update_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)

Update a support request attachment

Updates an existing support request attachment by its unique identifier.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::SupportRequestAttachmentsApi.new
tenant_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
support_request_attachment_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
opts = {
  api_version: 'api_version_example', # String | 
  x_api_version: 'x_api_version_example', # String | 
  support_request_attachment_update_dto: OpenapiClient::SupportRequestAttachmentUpdateDto.new # SupportRequestAttachmentUpdateDto | 
}

begin
  # Update a support request attachment
  result = api_instance.update_support_request_attachment_async(tenant_id, support_request_attachment_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->update_support_request_attachment_async: #{e}"
end
```

#### Using the update_support_request_attachment_async_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<EmptyEnvelope>, Integer, Hash)> update_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)

```ruby
begin
  # Update a support request attachment
  data, status_code, headers = api_instance.update_support_request_attachment_async_with_http_info(tenant_id, support_request_attachment_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <EmptyEnvelope>
rescue OpenapiClient::ApiError => e
  puts "Error when calling SupportRequestAttachmentsApi->update_support_request_attachment_async_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tenant_id** | **String** |  |  |
| **support_request_attachment_id** | **String** |  |  |
| **api_version** | **String** |  | [optional] |
| **x_api_version** | **String** |  | [optional] |
| **support_request_attachment_update_dto** | [**SupportRequestAttachmentUpdateDto**](SupportRequestAttachmentUpdateDto.md) |  | [optional] |

### Return type

[**EmptyEnvelope**](EmptyEnvelope.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/xml
- **Accept**: application/json, application/xml

